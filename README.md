# Projeto Bar e Restaurante - Sistema de Gestão

Este é um sistema de console para gerenciamento de um bar ou restaurante, desenvolvido em C# como um projeto de estudo para a disciplina de Programação Orientada a Objetos.

## Funcionalidades Principais

O sistema é dividido em quatro módulos principais, cada um com suas respectivas funcionalidades:

### Módulo de Contas e Pedidos
- **Abrir e Fechar Contas:** Gerencia o ciclo de vida de uma conta de cliente.
- **Adicionar e Remover Itens:** Permite registrar os produtos consumidos em uma conta.
- **Cálculo Automático:** Calcula o valor total da conta, incluindo uma taxa de serviço opcional de 10%.
- **Visualização de Contas:** Permite ver contas em aberto e contas já fechadas.
- **Faturamento Diário:** Exibe o total faturado no dia com base nas contas fechadas.

### Módulo de Mesas
- **CRUD completo:** Cadastro, Edição, Exclusão e Visualização de mesas.
- **Controle de Status:** Cada mesa possui um status de `Livre` ou `Ocupada`, que é atualizado automaticamente ao abrir ou fechar uma conta.
- **Regras de Negócio:** Garante que cada mesa tenha um número único e impede a exclusão se houver pedidos vinculados.

### Módulo de Garçons
- **CRUD completo:** Cadastro, Edição, Exclusão e Visualização de garçons.
- **Validações:** Valida o formato do CPF (`XXX.XXX.XXX-XX`) e garante que não existam CPFs duplicados.
- **Regras de Negócio:** Impede a exclusão de um garçom se ele estiver associado a algum pedido.

### Módulo de Produtos
- **CRUD completo:** Cadastro, Edição, Exclusão e Visualização de produtos do cardápio.
- **Regras de Negócio:** Garante que os nomes dos produtos sejam únicos e impede a exclusão se um produto estiver em algum pedido ativo ou fechado.
