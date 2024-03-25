função simularCorrida(velocidadeInicial, aceleracao, distancia, velocidadeMaxima, tempoMaximo):
    tempo = 0
    velocidade = velocidadeInicial
    
    enquanto verdadeiro:
        // Atualizar a velocidade e o tempo
        velocidade = velocidadeInicial + aceleracao * tempo
        
        // Verificar se a velocidade excede a velocidade máxima permitida
        se velocidade > velocidadeMaxima:
            velocidade = velocidadeMaxima
        
        // Calcular a distância percorrida até o momento
        distanciaPercorrida = (velocidadeInicial + velocidade) / 2 * tempo
        
        // Verificar se a distância percorrida é maior ou igual à distância total
        se distanciaPercorrida >= distancia:
            retornar tempo // Tempo necessário para completar a distância
        
        // Verificar se o tempo excede o tempo máximo permitido
        se tempo >= tempoMaximo:
            retornar "Tempo máximo excedido"
        
        // Incrementar o tempo para a próxima iteração
        tempo = tempo + 1