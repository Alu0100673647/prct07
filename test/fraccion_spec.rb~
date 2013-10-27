# Practica 6 Lenguajes y Paradigmas de la Programación
# Desarrollo Dirigido por el Comportamiento (Behavior Driven Development - BDD)
# Autores: Pedro Javier Núñez Rodríguez
#	   Constanza Leon Baritussio
# Fichero que contiene las pruebas de comportamiento para la clase Fraccion

require './fraccion.rb'

describe "Fraccion"do
	
	before :each do  # Esto se hara antes de cada bloque it
		@fraccion1 = Fraccion.new(3,9)		
		@fraccion2 = Fraccion.new(4,8)		
	end
	
	it "Debe existir un numerador" do
		@fraccion1.numerador.should be_a(Integer)
	end

    it "Debe existir un denominador" do
        @fraccion1.denominador.should be_a(Integer)
    end

	it "Debe de estar en su forma reducida" do
		@fraccion1.numerador.should == 1
		@fraccion1.denominador.should == 3
	end

	it "Se debe invocar al metodo num() para obtener el numerador" do
		@fraccion1.num().should == 1
	end                                         

	it "Se debe invocar al metodo denom() para obtener el denominador" do
		@fraccion1.denom().should == 3
	end
	
	it "Se debe mostar por la consola la fraccion de la forma: a/b, donde a es el numerador y b el denominador" do
	   @fraccion1.to_s.should == "1/3"
	end
	
	it "Se debe mostar por la consola la fraccion en formato flotante" do
	   @fraccion1.to_f.should == 1.to_f / 3.to_f
	end

	it "Se debe comparar si dos fracciones son iguales con ==" do
	   @fraccion1.should == Fraccion.new(1,3)
	end
	
	it "Se debe calcular el valor absoluto de una fraccion con el metodo abs" do
	   Fraccion.new(-1,3).abs.should == @fraccion1
	end
	
	it "Se debe calcular el reciproco de una fraccion con el metodo reciprocal" do
	   @fraccion1.reciprocal.should == Fraccion.new(3,1)
	end
	
	it "Se debe calcular el opuesto de una fraccion con -" do
	   Fraccion.new(-1,3).should == -@fraccion1
	end
	
	it "Se debe sumar dos fracciones con + y dar el resultado de forma reducida" do
	   (@fraccion1 + @fraccion2).should == Fraccion.new(5,6)
	end
	
	it "Se debe restar dos fracciones con - y dar el resultado de forma reducida" do
	   (@fraccion1 - @fraccion2).should == Fraccion.new(-1,6)
	end
	
	it "Se debe multiplicar dos fracciones con * y dar el resultado de forma reducida" do
	   (@fraccion1 * @fraccion2).should == Fraccion.new(1,6)
	end
	
	it "Se debe dividir dos fracciones con / y dar el resultado de forma reducida" do
	   (@fraccion1 / @fraccion2).should == Fraccion.new(2,3)
	end
	
	it "Se debe calcular el resto dos fracciones con % y dar el resultado de forma reducida" do
	    (@fraccion1 % @fraccion2).should == Fraccion.new(1,1)
	end

	it "Se debe de poder comprobar si una fracion es menor que otra" do
                (@fraccion1 < @fraccion2).should == true          
	end
	
	it "Se debe de poder comprobar si una fracion es mayor que otra" do
		(@fraccion1 > @fraccion2).should == false
	end
	
	it "Se debe de poder comprobar si una fracion es menor o igual que otra" do
		(@fraccion1 <= @fraccion2) == true
	end
	
	it "Se debe de poder comprobar si una fracion es mayor o igual que otra" do
	(@fraccion1 >= @fraccion2).should == false
	end
	
end

                                                                                                               
