# Rectangle (Cálculo de Retângulo)

Este é um programa de console simples, escrito em Java, focado nos princípios de Programação Orientada a Objetos (POO). O programa solicita ao usuário a largura e a altura de um retângulo e, em seguida, calcula e exibe sua área, perímetro e diagonal.

## Funcionalidades

  * **Entrada de Dados:** Solicita ao usuário que insira a largura (`width`) e a altura (`height`) do retângulo.
  * **Cálculo de Área:** Possui um método (`area`) que retorna `largura * altura`.
  * **Cálculo de Perímetro:** Inclui um método (`perimeter`) que retorna `2 * (largura + altura)`.
  * **Cálculo de Diagonal:** Utiliza o Teorema de Pitágoras em um método (`diagonal`) para retornar `Math.sqrt(width * width + height * height)`.
  * **Exibição Formatada:** Imprime os resultados no console com duas casas decimais.

## Estrutura do Repositório

O projeto está organizado da seguinte forma:

```
/
├── src/                      # Pasta contendo o código-fonte .java
│   ├── application/
│   │   └── Program.java      # Classe principal (main) que executa a aplicação
│   └── entities/
│       └── rectangle.java    # Classe de entidade que define o Retângulo
│
├── bin/                      # Pasta contendo os arquivos .class compilados
│   ├── application/
│   │   └── Program.class
│   └── entities/
│       └── rectangle.class
│
└── README.md                 # Este arquivo de descrição
```

## Como Usar

Este é um projeto de console Java. Para executá-lo, você precisará ter o Java Development Kit (JDK) instalado e configurado.

1.  **Compilação (Opcional, se já não estiver compilado):**
    Navegue até a raiz do projeto e compile os arquivos-fonte, direcionando a saída para a pasta `bin`:

    ```bash
    javac -d bin src/application/Program.java src/entities/rectangle.java
    ```

2.  **Execução:**
    A partir da raiz do projeto, execute a classe `Program` que está dentro da pasta `bin`:

    ```bash
    java -cp bin application.Program
    ```

3.  **Interação com o Programa:**
    O console solicitará as seguintes informações:

      * `Enter rectangle width and height:` (Insira a largura e a altura do retângulo)

    Após inserir os dois valores (separados por espaço ou Enter), o programa exibirá os resultados:

      * `AREA = [valor]`
      * `PERIMETER = [valor]`
      * `DIAGONAL = [valor]`

## Observações

  * **Formato de Números:** O programa está configurado com `Locale.US`. Isso significa que, ao inserir valores decimais (como `10.5`), você deve usar o **ponto** (`.`) como separador, e não a vírgula.
