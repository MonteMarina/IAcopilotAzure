**Desafio: Explorando os Recursos de IA Generativa com Copilot e OpenAI**


Ao utilizar o Copilot, percebi que durante as interações de teste, ele prontamente oferece novas sugestões de interações relacionadas ao tema em questão, tornando-se assim uma ferramenta extremamente dinâmica e repleta de possibilidades. Sua capacidade de gerar ideias, completar tarefas e facilitar o aprendizado é altamente notável. As várias vertentes que podem ser exploradas na IA Generativa me impressionaram, desde a rápida automatização de tarefas até a criação de imagens, músicas, textos e, especialmente, a geração e o aprimoramento de código. Em resumo, o Copilot é um grande suporte criativo.

Como foi o caso abaixo:
![image](https://github.com/MonteMarina/IAcopilotAzure/assets/154125061/40aceb57-28b6-4a92-b0bb-8a1fc4d88dab)

using System;
using System.Collections.Generic;
using System.Linq;

namespace EstacionamentoApp
{
    public class Estacionamento
    {
        private decimal precoInicial;
        private decimal precoPorHora;
        private List<string> veiculos;

        // Construtor da classe
        public Estacionamento(decimal precoInicial, decimal precoPorHora)
        {
            this.precoInicial = precoInicial;
            this.precoPorHora = precoPorHora;
            this.veiculos = new List<string>();
        }

        // Método para adicionar um veículo ao estacionamento
        public void AdicionarVeiculo()
        {
            Console.WriteLine("Digite a placa do veículo para estacionar:");
            string placa = Console.ReadLine();

            if (veiculos.Any(v => v.Equals(placa.ToUpper())))
            {
                Console.WriteLine("Já existe um veículo com essa placa.");
            }
            else
            {
                veiculos.Add(placa);
                Console.WriteLine("Veículo estacionado com sucesso!");
            }
        }

        // Método para remover um veículo do estacionamento
        public void RemoverVeiculo()
        {
            // Implemente a lógica para remover um veículo
        }

        // Método para listar os veículos estacionados
        public void ListarVeiculos()
        {
            // Implemente a lógica para listar os veículos
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            // Exemplo de uso
            Estacionamento estacionamento = new Estacionamento(precoInicial: 5.0m, precoPorHora: 2.0m);
            estacionamento.AdicionarVeiculo();

            // Mais funcionalidades podem ser adicionadas conforme necessário
        }
    }
}

![image](https://github.com/MonteMarina/IAcopilotAzure/assets/154125061/c2f39c1e-571d-4649-8dd3-90bc3a663cdd)



