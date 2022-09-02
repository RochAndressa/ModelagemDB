# ModelagemDBOficina
Desafio Bootcamp DIO oficina

#### Objetivo:
Criar o esquema conceitual para o contexto de oficina com base na narrativa fornecida.

#### Narrativa:
 - Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica.
 - Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões periódicas.
 - Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com a data de entrega.
 - A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra.
 - O valor de cada peça também irá compor a OS, o cliente autoriza a execução dos serviços.
 - A mesma equipe avalia e executa os serviços.
 - Os mecânicos possuem código, nome, endereço e especialidade.
 - Cada OS possui: nº, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

#### Como foi feita a modelagem:
 - O relacionamento de cliente com OS de 1:n ( onde ele pode ter mais de uma OS vinculada a ele, mas a OS só tera um cliente vinculado a ela)
 - O cliente também tem relacionamento com veiculo, onde poderá ser registrado mais de um veículo por cliente.
 - A OS está relacionada aos serviços através da definição dos serviços e também relacionada a mecânicos através da equipe de mecânicos.
 - As peças estão relacionadas a OS e descritas nomeadamente cada uma por OS.
 - O serviço só é executado com autorização prévia do cliente descrita na OS.

