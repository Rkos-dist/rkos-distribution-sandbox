# Aviso de coleta de dados do servidor RKOS (instalacao)

> RASCUNHO v0.1 - NAO e documento juridico. Escrito pelo planejamento do projeto para ser revisado pelo dono e depois por advogado.
> Trechos entre [A PREENCHER] precisam de dado do dono. Trechos com [ADVOGADO] precisam de parecer juridico.
> Versao: 0.1 (rascunho) - Atualizado em 2026-10-23 - Quando for publicado, a versao passa a numerar 1.0, 1.1...

O RKOS instalado no seu servidor se comunica com o License Manager e com o repositorio de distribuicao apenas para licenciamento e atualizacao.

## O que sai do seu servidor
- Na ativacao: chaves publicas da instalacao, **hashes** do hardware (placa, BIOS, identificador do sistema - nao os numeros em claro), versao do RKOS, sistema operacional, codigo de ativacao.
- Periodicamente (melhor esforco, agregado): estado da licenca, versao instalada, resultado de atualizacoes, estado de integridade, data da ultima verificacao.
- Trafego de acesso remoto passa pelo tunel Cloudflare contratado para a sua instalacao.

## O que NAO sai
Nada do conteudo do sistema: clientes finais, equipe, eventos, estoque, financeiro, documentos, fotos, conversas, planilhas ou backups.

## Arquivos que seu servidor baixa
Licenca selada para o seu servidor, chaves de atualizacao seladas, pacotes de atualizacao cifrados e assinados, manifestos e este tipo de documento legal. O conteudo e legivel apenas pelo RKOS correto.

## Seus controles
Voce ve no sistema (Configuracoes > Licenca) o historico de verificacoes. Dados do portal podem ser exportados ou excluidos pelo portal. [ADVOGADO: conferir coerencia com a Politica de Privacidade]
