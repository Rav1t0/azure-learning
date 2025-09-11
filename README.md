# azure-learning
  Este repositório contém o resumo, anotações, conceitos, dicas e imagens sobre o uso do Azure, dessa vez, com foco prático no processo de configuração de uma instância de Banco de Dados.

## Introdução
  Este repositório foi elaborado, como parte do desafio final do módulo 1 do bootcamp "Microsoft Azure AZ-900" na DIO.

## Conceitos
  Inicialmente, vale lembrar que apenas o modelo On-Premise o cliente tem total responsabilidade.

  A respeito dos modelos, IaaS, PaaS e SaaS, para os serviços de:
  - Hosts físicos
  - Redes físicas
  - Datacenter físico
  Em todos os modelos, a responsabilidade é transferida para o provedor de nuvem.

  E para os serviços:
  - Informações e dados
  - Dispositivos
  - Contas e identidades
  Em todos os modelos, a responsabilidade é sempre retida pelo cliente.

  Entre essas duas extremidades, segue as descrições e demais responsabilidades de cada modelo:

  - IaaS (Infraestrutura como Serviço)   ->    O cliente gerencia quase tudo, exceto os serviços físicos citados acima, e não há responsabilidades compartilhadas.
  - PaaS (Plataforma como Serviço)       ->    O cliente foca nas aplicações, o provedor cuida da infra e da plataforma.
  - SaaS (Software como Serviço)         ->    O cliente só usa a nuvem, pagando de acordo com o uso, em um modelo de assinatura (ex.: Microsoft 365).

## Resource Group
  - O que são:
    
    Grupo de recursos, um agrupamento lógico onde pode ser agrupado todos os recursos, de forma organizada e subdividida.

## Máquinas Virtuais no Azure
  - O que são:
    
    Computadores baseados em software, criados virtualmente, que executam os aplicativos e sistema operacional em servidores físicos hospedados na nuvem.
    
  - Quando utilizar:
    
    Para testes de ambiente, simulações, rodar aplicações específicas sem a necessidade de comprar hardwares físicos.
    
  - Valores de imagens de VMs:
    
    Durante o laboratório e prática, percebi que há diversos valores de imagens, que mudam de acordo com: região que será hospedado e executado,
    Sistema operacional escolhido e também depende da quantidade de CPU, RAM   e disco.

## Banco de Dados SQL no Azure
  - Passos principais para criar a instância:
    
    Selecionar serviço de SQL Database, acionar a opção de criar e seguir com o preenchimento do nome e criação do Servidor que terá o banco alocado, isso detalhará o valor do banco especificado.
    
  - Configurações básicas:
    
    Nome do banco, servidor escolhido, local do servidor, contrato de backup, a rede do banco, configurações de segurança, como Windows Defender e tags.

## Dicas
  - Dicas práticas:
    
    É importante sempre criar um Resource Group separado para testes e laboratórios. Assim basta excluir o RG e limpar todos os recursos sem deixar nada ativo ou criado sem necessidade.
  
  - Pontos de atenção:
    
    Atenção a opções como: Deletar ip público ao deletar VM. Opção de gerar IP Público ou não, no momento de criação da VM, para ter certeza se será necessário VPN para acesso ou não.\
    Importante revisar valores estabelecidos nas criações de serviços e revisar as opções dentro de cada criação, como rede, segurança, etc.
  
  - Erros comuns a evitar:
    
    Criar recursos em regiões diferentes sem perceber (isso pode aumentar latência e custo). Ao deletar uma VM, por exemplo, ter certeza de não deixar recursos ativos sem deletar e gerando cobranças desnecessárias.

## Conclusão  
  Este desafio ajudou a reforçar conceitos de modelos de serviço em nuvem, além de colocar em prática a criação de recursos básicos como VMs e SQL Database no Azure.
  Também foi possível entender melhor, custos, responsabilidades e boas práticas para organizar e encerrar recursos corretamente.

## Referências
  - [Documentação Oficial do Azure](https://learn.microsoft.com/azure)
  - [Quickstart: SQL Database](https://learn.microsoft.com/azure/azure-sql/database/single-database-create-quickstart)
  - Materiais da DIO
