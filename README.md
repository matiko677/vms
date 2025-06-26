# vms
nem todas as regiões possuem todas as familias de máquinas

armazenamento de vm
cada vm do azure tem dois ou mais discos
disco do so
disco temporario(nem todos os SKUs tem um, o conteudo pode ser perdido
discos de dados
o disco temporário perde tudo quando reiniciado

backup da vm é configurado e gerenciado pelo usuárioQual é a principal vantagem de usar o Azure Bastion para acesso remoto a uma máquina virtual? 
Ele fornece um acesso seguro sem a necessidade de expor as portas RDP ou SSH à internet. 

máquina em produção- alta disponibilidade e replicação para outras regiões e backups do seu estadoDurante o processo de criação de uma máquina virtual no Azure, qual é a opção que a Microsoft não recomenda para ambientes de produção? 
Usar o modelo Spot devido à possibilidade de desalocação da máquina 

apesar de estar na nuvem ainda estamos propensos a falhar de hardware no rack do provider, quando ocorre isso a microsoft faz uma migração às pressas 

evento de manutencao-microsoft avisa sobre uma manutenção planejada preventiva que deverá ser feita no rack da máquina virtual 

conjuntos de disponibilidade- configuração de uma redundância a nível de datacenter, de forma que impede que todas as suas máquinas estejam no mesmo rack e aí se esse um rack tiver alguma falha, algum dos seus servições vão pode ser facilmnente migrados para outra vm em outro hack que já vai ter um ambinete pré configurado para receber seu sistema
domínios com falha-define quantos racks você quer que hospedem as suas vms
domínio de atualização-define quantas paridades entre racks existem, como se fossem hospedeiros para receberem a estrutura identica a da vm do rack que teve algum problema

possibilidade de replicação do conjunto de disponibilidade para zonas de disponibilidade

dimensionamento vertical(escala)- aumento e redução de escala, processo de aumento ou diminuição dos requisitos de uma carga de trabalho
dimensionamento escala horizontal-elasticidade, adaptação de acordo com as necessidades 

é possível setar config para o dimensionamento automatico relativo a escala horizontal de maneira a limitar crescimento e o decrescimoQuando a Microsoft utiliza uma manutenção planejada em máquinas virtuais no Azure, o que os administradores devem fazer para evitar downtime inesperado? Os administradores devem mover as máquinas para outro local ou grupo de recursos conforme indicado pela Microsoft antes da manutenção. 

é possível desanexar o disco de uma vm para fazer backuop em outra vm por exemplo

opções de disponibilidade
zonas de disponibilidade- separar o recurso em datacenters diferentes, uma vm por zona, criação de mais de uma vm 
scale set- caso de uma época com produção atipica, necessidade de aumento dos recursos proporcional a aumento da produção
availability set- evitar problemas relativos a indisponibilidade dos serviços com os recursos fault domain e update domain
