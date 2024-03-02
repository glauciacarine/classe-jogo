// Definição da classe Heroi
class Heroi {
    constructor(nome, idade, tipo) {
        this.nome = nome;
        this.idade = idade;
        this.tipo = tipo;
    }

    // Método para realizar o ataque
    atacar() {
        let ataque;
        switch (this.tipo) {
            case "mago":
                ataque = "usou magia";
                break;
            case "guerreiro":
                ataque = "usou espada";
                break;
            case "monge":
                ataque = "usou artes marciais";
                break;
            case "ninja":
                ataque = "usou shuriken";
                break;
            default:
                ataque = "usou um ataque desconhecido";
        }
        console.log(`O ${this.tipo} atacou usando ${ataque}`);
    }
}

// Exemplo de uso da classe Heroi
let heroi1 = new Heroi("Aragorn", 35, "guerreiro");
heroi1.atacar(); // Saída: O guerreiro atacou usando espada

let heroi2 = new Heroi("Gandalf", 120, "mago");
heroi2.atacar(); // Saída: O mago atacou usando magia
