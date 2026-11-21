# Contrato de Licenca de Uso do RKOS (EULA)

> RASCUNHO v0.1 - NAO e documento juridico. Escrito pelo planejamento do projeto para ser revisado pelo dono e depois por advogado.
> Trechos entre [A PREENCHER] precisam de dado do dono. Trechos com [ADVOGADO] precisam de parecer juridico.
> Versao: 0.2 (rascunho) - Atualizado em 2026-10-30 (clausula 6-A: recuperacao de backup pelo suporte) - Quando for publicado, a versao passa a numerar 1.0, 1.1...

## 1. Objeto
Licenca nao exclusiva, intransferivel e revogavel de uso do software RKOS (e suas atualizacoes durante a vigencia), na instalacao e no hardware identificados na licenca, para as finalidades internas do cliente, conforme os direitos do plano contratado (modulos, usuarios, instalacoes, atualizacoes).
Servicos relacionados: instalacao e suporte; o servidor e cedido em comodato conforme o Termo de Comodato (anexo). [ADVOGADO]

## 2. Como a licenca funciona (transparencia tecnica)
- A licenca e um arquivo assinado e cifrado, valido apenas para a instalacao e hardware ativados, renovado automaticamente a cada ciclo (mensal: todo mes; anual: a cada 2 meses) enquanto a assinatura estiver em dia.
- O RKOS verifica a licenca localmente. Sem acesso ao repositorio de licencas, o sistema continua funcionando durante a tolerancia de **30 dias** apos o vencimento do ciclo; apos isso, o acesso e bloqueado ate que uma licenca valida seja recebida. Nenhum dado do cliente e apagado. Administradores podem exportar um backup cifrado mesmo com o sistema bloqueado.
- Atualizacoes sao baixadas e instaladas automaticamente na janela de manutencao, com backup previo e reversao automatica em caso de falha.
- O RKOS verifica a integridade do proprio software e, se detectar alteracao, exibe aviso e pode restringir o uso (ver clausula 5).

## 3. Direitos e limites
Numero de usuarios, instalacoes, modulos e versao conforme o plano. Trocar de hardware: [1 vez por trimestre] pelo portal; acima disso, mediante aprovacao do suporte.

## 4. O cliente nao pode
Copiar, sublicenciar, revender, emprestar ou ceder a licenca; usar em hardware nao licenciado; contornar, desativar ou enganar o licenciamento ou a verificacao de integridade (inclusive adulterando relogio, arquivos ou chaves); descompilar, fazer engenharia reversa ou tentar extrair codigo-fonte ou chaves, salvo nos limites imperativos da lei; remover avisos de propriedade. [ADVOGADO]

## 5. Integridade rompida
Se o RKOS detectar que o software, a licenca ou o ambiente foram alterados fora dos meios oficiais, podera: registrar o evento, avisar os administradores, comunicar o estado ao fornecedor (sem conteudo do sistema) e, apos o prazo de observacao previsto, restringir o acesso ate verificacao pelo suporte. [ADVOGADO: validade e aviso previo]

## 6. Propriedade e dados
O software e do fornecedor. Os dados inseridos no sistema sao do cliente, que e o controlador. O fornecedor so acessa dados do cliente quando solicitado ao suporte e com autorizacao, como operador, inclusive na recuperacao de backup da clausula 6-A. [ADVOGADO: LGPD]

## 6-A. Recuperacao de backup pelo suporte (opcional)
- Os backups do RKOS sao cifrados com a senha escolhida pelo cliente ao cria-los; sem essa senha, ninguem os abre, nem o fornecedor.
- O cliente pode ATIVAR a recuperacao pelo suporte. Com ela ativa, cada backup criado a partir de entao tambem recebe uma segunda chave, que so o fornecedor consegue usar (chave privada guardada sob custodia do fornecedor).
- Finalidade unica: devolver ao cliente os dados dele quando a senha do backup nao estiver disponivel, por exemplo avaria do servidor ou fim do contrato (clausula 9), sem que o cliente precise contratar mais tempo de uso so para exportar os dados.
- Uso: somente a pedido de um responsavel pelo cliente, com confirmacao de identidade, e somente sobre o arquivo de backup que o cliente entregar ao suporte. O fornecedor abre o backup apenas para gerar os arquivos de entrega (planilhas com os dados e os anexos), entrega-os somente ao cliente e nao guarda copia apos a entrega. Cada uso e registrado (quem, quando, qual arquivo). O fornecedor nao acessa o servidor nem os dados do cliente em nenhuma outra situacao por causa deste recurso.
- Decisao: a escolha e feita por um administrador do sistema num aviso obrigatorio no primeiro acesso, que explica o recurso e linka a Politica de Privacidade. O aceite nesse aviso integra este contrato. O administrador pode ativar ou desativar a qualquer momento em Configuracoes > Sistema > Backup (com senha e segundo fator, quando ativo); cada decisao e registrada com a versao do aviso aceito, data, usuario e IP.
- Desativada: os backups ficam protegidos apenas pela senha do cliente. Se a senha for perdida ou o servidor sofrer avaria, o fornecedor NAO consegue recuperar nem liberar os dados, e nao responde por essa perda.
- A escolha vale para os backups criados a partir dela; um backup criado com a recuperacao ativa continua recuperavel ate ser excluido pelo cliente.
[ADVOGADO: natureza do aceite eletronico, LGPD (operador, finalidade, minimizacao), responsabilidade na entrega]

## 7. Pagamento, atraso, suspensao e cancelamento
Conforme o documento "Cancelamento e Reembolso". Falta de pagamento interrompe a publicacao de renovacoes; o sistema segue ate o fim do ciclo vigente e da tolerancia.

## 8. Garantia e responsabilidade
[ADVOGADO: garantia limitada, exclusoes, limite de responsabilidade, parada operacional, forca maior, backups sob responsabilidade do cliente.]

## 9. Vigencia e rescisao
Vigora enquanto a assinatura estiver ativa. Rescisao por descumprimento, com os efeitos descritos. Apos o termino, o cliente mantem seus dados e pode exporta-los conforme clausula 2; com a recuperacao pelo suporte ativa (clausula 6-A), ou informando a senha de um backup, pode tambem pedir ao suporte a entrega dos dados em planilhas, sem precisar pagar novo periodo de uso. [A PREENCHER: prazo para o pedido e eventual custo do servico]

## 10. Acesso remoto
O fornecedor pode disponibilizar endereco publico e tunel gerenciado para o servidor do cliente; o endereco e as credenciais do tunel sao entregues dentro da licenca e podem ser removidos em caso de cancelamento, revogacao ou fim da tolerancia.

## 11. Lei e foro
Lei brasileira. Foro: [ADVOGADO/A PREENCHER].
