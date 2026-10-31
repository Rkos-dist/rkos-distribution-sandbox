# Politica de Privacidade (LGPD) - RKOS License Manager e RKOS

> RASCUNHO v0.2 - NAO e documento juridico. Escrito pelo planejamento do projeto para ser revisado pelo dono e depois por advogado.
> Trechos entre [A PREENCHER] precisam de dado do dono. Trechos com [ADVOGADO] precisam de parecer juridico.
> Versao: 0.3 (rascunho) - Atualizado em 2026-10-30 (recuperacao de backup pelo suporte) - Quando for publicado, a versao passa a numerar 1.0, 1.1...

## 1. Quem somos
[RAZAO SOCIAL], CNPJ [A PREENCHER], controladora dos dados do portal. Encarregado (DPO): [NOME/E-MAIL].

## 2. Quais dados tratamos, para que e com qual base legal
| Dado | Finalidade | Base legal [ADVOGADO] | Retencao |
|---|---|---|---|
| Nome/razao social, e-mail, telefone, documento (CPF/CNPJ) | Criar conta, contratar, cobrar, emitir documentos fiscais futuros | Execucao de contrato; obrigacao legal | Enquanto houver conta + prazo legal |
| Senha | Autenticacao (guardamos so o hash) | Execucao de contrato | Ate exclusao da conta |
| Segundo fator (TOTP) | Seguranca da conta | Legitimo interesse / contrato | Ate desativar |
| Pagamentos (valor, data, status, identificador no provedor) | Cobranca, conciliacao, comissoes | Execucao de contrato; obrigacao legal | Prazo fiscal/contabil [A PREENCHER] |
| IP e navegador (mascarados quando possivel), logs de acesso | Seguranca, prevencao de fraude, Marco Civil (guarda de registros) | Obrigacao legal; legitimo interesse | [A PREENCHER: 6 meses a 1 ano] |
| Identificador da instalacao, hashes de hardware, versao, SO, estado da licenca/integridade | Licenciar, evitar copia indevida, suporte | Execucao de contrato; legitimo interesse | Enquanto houver licenca |
| Dados de parceiros (nome, documento, chave PIX, vendas, comissoes) | Pagar comissoes | Execucao de contrato; obrigacao legal | Prazo fiscal |
| CPF do pagador de BOLETO | Emitir o boleto e gerar as cobrancas de renovacao | Execucao de contrato | Guardado CIFRADO (chave mestra do LM), usado so para gerar cobrancas; APAGADO ao cancelar a assinatura |
| Hash (irreversivel) do documento do pagador e da combinacao IP + navegador do cadastro | Prevencao de fraude em indicacoes (auto-indicacao de parceiro): so comparamos hashes, nao guardamos o numero nem o navegador em claro | Legitimo interesse | Enquanto durar a comissao + prazo prescricional |
| Cupom usado e origem da venda (parceiro por link ou cupom) | Aplicar desconto e calcular comissao | Execucao de contrato; legitimo interesse | Prazo fiscal |
| Conteudo de um backup do RKOS entregue pelo cliente ao suporte (so com a recuperacao pelo suporte ativada, ou com a senha informada pelo cliente) | Unicamente gerar e entregar ao proprio cliente os dados dele em planilhas e anexos (avaria do servidor, fim de contrato) | Execucao de contrato (como operador, por instrucao do cliente controlador) | Somente durante a geracao da entrega; nenhuma copia guardada depois. Fica so o registro do uso (quem, quando, qual arquivo) |
| Decisao sobre a recuperacao de backup pelo suporte (ativar/desativar, versao do aviso, data, usuario, IP) | Prova do consentimento/contrato | Execucao de contrato; legitimo interesse | Enquanto durar a relacao + prazo prescricional |
| Aceites de documentos (versao, data, IP) | Prova de consentimento/contrato | Legitimo interesse; obrigacao legal | Enquanto durar a relacao + prazo prescricional |

## 3. O que NAO tratamos
Nao temos acesso ao conteudo do sistema do cliente (eventos, clientes finais, equipe, financeiro, etc.): ele fica no servidor do cliente. Unica excecao: a recuperacao de backup pelo suporte, que o administrador do cliente escolhe ativar ou nao (e pode mudar quando quiser). Mesmo ativa, so abrimos um backup que o proprio cliente nos entregar, a pedido dele, para devolver os dados a ele (ver EULA, clausula 6-A). Com ela desativada, nao conseguimos abrir os backups em nenhuma hipotese. Nao guardamos dados de cartao (ficam no provedor de pagamento).

## 4. Compartilhamento
Provedores de pagamento (Mercado Pago, Efi Bank), Cloudflare (acesso remoto e DNS), GitHub (distribuicao de arquivos cifrados e assinados, sem dados pessoais legiveis), servico de envio de e-mail [A PREENCHER]. Autoridades quando exigido por lei. Parceiros recebem apenas o minimo (que houve uma venda, valor e comissao; sem dados pessoais do cliente). [ADVOGADO: transferencia internacional]

## 5. Seus direitos
Confirmacao e acesso, correcao, anonimizacao/bloqueio/eliminacao, portabilidade, informacao sobre compartilhamento, revogacao de consentimento, oposicao. Pedidos pelo portal (Conta > Privacidade) ou para [E-MAIL DO DPO]; resposta em ate [15] dias.

## 6. Seguranca
Senhas com hash forte, 2FA, criptografia em transito, chaves em cofre cifrado, auditoria de acessos, minimo de dados, backups cifrados. Incidentes serao comunicados conforme a LGPD. [ADVOGADO: prazos e canal]

## 7. Cookies
Apenas cookies essenciais (sessao, seguranca) e o cookie de origem de parceiro (ate 60 dias) quando voce chega por um link de indicacao. [A PREENCHER: aviso de cookies]

## 8. Criancas
O servico e destinado a empresas; nao coletamos dados de menores de forma intencional.

## 9. Mudancas
Esta politica e versionada; mudancas relevantes sao avisadas e a versao aceita fica registrada.
