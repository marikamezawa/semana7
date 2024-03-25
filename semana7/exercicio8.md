Classe FormaGeometrica:
    Atributos:
        - cor

    Método Construtor(cor):
        Define o valor do atributo cor com o valor passado como parâmetro.

    Método CalcularArea():
        # Implementação genérica para cálculo de área, a ser sobrescrita pelas subclasses.



Classe Retangulo derivada de FormaGeometrica:
     Atributos:
         - base
         -  altura

    Método Construtor(cor, base, altura):
        // Define os valores do atributo base e altura que pertence a esta classe
        // Define também o atributo herdado da classe FormaGeometrica

    Método CalcularArea():
	    retornar base * altura

Classe Circulo derivada de FormaGeometrica:
	 Atributos: 
         - raio

    Método Construtor(cor, raio):
	    // Define o valor do atributo raio que pertence a esta classe
        // Define também o atributo herdado da classe FormaGeometrica

    Método CalcularArea():
	    retornar pi * raio^2

