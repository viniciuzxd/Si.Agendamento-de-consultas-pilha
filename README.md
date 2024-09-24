# Sistema de Agendamento de Consultas

Este projeto é um sistema de agendamento de consultas médicas e odontológicas, desenvolvido em Java. Ele permite que os usuários agendem consultas, notifiquem chegadas e gerenciem informações de pacientes.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

- `App`: Contém a classe principal `App.java` que executa o sistema.
- `Entidades`: Contém as classes de entidades como `Consulta`, `ConsultaMedica`, `ConsultaOdontologica` e `Paciente`.
- `Repositorios`: Contém as classes de repositórios como `RconsultaMedica` e `RconsultaOdontologica`.
- `Servicos`: Contém as classes de serviços como `ServicoConsultaMedica`, `ServicoConsultaOdontologica` e `ServicoNotificacao`.

## Pilha de Médicos

A pilha de médicos (`RpilhaMedico`) é utilizada para gerenciar a lista de médicos disponíveis para consultas. Ela permite adicionar (empilhar) e remover (desempilhar) médicos, além de verificar o médico no topo da pilha e o tamanho da pilha.

### Localização da Pilha no Código

A pilha de médicos é instanciada e utilizada no arquivo `Si.Agendamento/src/App/App.java` nas seguintes linhas:

- **Linha 18**: Instanciação da pilha `RpilhaMedico`.
- **Linha 55**: Utilização do método `empilhar` da pilha `RpilhaMedico`.

### Exemplo de Uso

No método `main` da classe `App`, a pilha de médicos é utilizada para empilhar médicos quando uma consulta médica é agendada.
