#Todos los ejercicios se realizaron dentro de un collab, la libreria esta escrita en el primer bloque de codigo

#El resto de ejercicios estan puestos cada uno en un bloque de codigo

#Quantum-sim: simulador y ejercicios (Capítulo 4)

Repositorio con la implementación en Python / Jupyter de:
- Simulador del sistema cuántico de la sección 4.1
- Retos de programación del capítulo 4: ejercicios 4.3.1, 4.3.2, 4.4.1 y 4.4.2


#Discusión de ejercicios 4.5.2 y 4.5.3 

-En el Ejercicio 4.5.2, se plantea escribir el vector de estado genérico para un sistema de dos partículas con espín, y luego generalizarlo para un sistema de n partículas.
Para dos partículas, el espacio de Hilbert total se construye como el producto tensorial de los espacios individuales:
                                    Htotal​=H1​⊗H2​.
                                    
Si cada partícula tiene dos estados posibles (por ejemplo, 
∣0⟩ y ∣1⟩, el sistema total puede representarse como una combinación lineal de los cuatro estados base:
                            |ψ⟩= c00​ ∣00⟩ + c01 ​∣01⟩ + c10 ​∣10⟩ + c11​ ∣11⟩
                            
donde los coeficientes 𝑐𝑖𝑗 son complejos y deben satisfacer la condición de normalización ∑∣𝑐𝑖𝑗∣^2=1
Para un sistema de n partículas, el vector de estado es un elemento del espacio 𝐶^(2𝑛), y puede representarse como una superposición de los 2^𝑛
estados base posibles. Esta construcción es fundamental, ya que es la base teórica para los registros cuánticos en computación cuántica.


-En el Ejercicio 4.5.3, se analiza la separabilidad del estado:

            ∣𝜙⟩= ∣𝑥0⟩ ⊗ ∣𝑦1⟩ + ∣𝑥1⟩ ⊗ ∣𝑦1⟩
            
Este estado no puede escribirse como un único producto tensorial de dos vectores (uno en cada subespacio), por lo que no es separable. Esto implica que es un estado entrelazado, 
lo que significa que las dos partículas no pueden describirse de manera independiente. Este tipo de estados es esencial en fenómenos puramente cuánticos como el entrelazamiento
y la no localidad, y son recursos clave en protocolos de teleportación cuántica y en el poder de cómputo de los algoritmos cuánticos
