# Extrator de metadados · RI UERN

Programa gratuito para **Windows e Linux** que ajuda a cadastrar teses, dissertações e TCCs no
Repositório Institucional da UERN (DSpace). Você arrasta a dissertação/TCC e o Termo de
Autorização (PDF) e ele mostra, **pronto para copiar e colar**, cada campo do formulário:
Autor, Título, Data de emissão, Citação, Tipo, Idioma, Palavras-chave e Resumo.

> É uma ferramenta de apoio: **confira os campos marcados como REVISAR** antes de colar no DSpace.

## Baixar
Acesse **[Releases → versão mais recente](../../releases/latest)** e baixe:

| Sistema | Arquivo |
|---|---|
| **Windows 10/11** | `instalar-extrator-ri-uern-X.Y.Z.exe` |
| Linux (64 bits) | `extrator-ri-uern-X.Y.Z-linux-x64.tar.gz` |

## Instalar no Windows
1. Baixe o `.exe` e abra. **Não pede senha de administrador**; instala só para o seu usuário.
2. Se aparecer **"O Windows protegeu o computador"**, clique em **Mais informações → Executar assim mesmo**.
   (Acontece porque o instalador ainda não tem assinatura digital paga. O arquivo é o mesmo publicado aqui;
   o código de verificação SHA-256 está nas notas de cada versão.)
3. Conclua o instalador. Ele cria um atalho na Área de Trabalho e no Menu Iniciar.

Se o antivírus reclamar, é um falso positivo comum em programas empacotados em Python. Peça à TI para liberar.

## Usar no Linux
Extraia o `.tar.gz` e execute `extrator-ri-uern/extrator-ri-uern`. Não há instalação.

## Como usar
1. Abra o programa e **arraste** a dissertação/TCC e o Termo de Autorização (o Termo é opcional).
2. Clique em **Extrair metadados**.
3. Revise os campos. Cada um é editável; a **Citação** acompanha o Autor e o Título.
4. Clique em **Copiar** ao lado do campo e cole no formulário do DSpace.
5. **Novo item** limpa tudo para o próximo cadastro.

## Atualizações
No Windows, ao abrir, o programa verifica se há versão nova. Se houver, ele mostra
**"Atualizando…"**, baixa a atualização, confere a integridade (SHA-256), fecha e **abre sozinho já atualizado**.
Precisa de internet; sem internet o programa funciona normalmente na versão atual.
No Linux, a troca é manual (baixe o novo `.tar.gz`).

## Privacidade
- A extração acontece **no seu computador**. Os PDFs **não são enviados** a nenhum serviço.
- O programa só acessa a internet para ler um pequeno arquivo de avisos de versão e, quando há
  atualização, para baixá-la daqui.

## Algo deu errado?
Se aparecer um erro, clique em **Copiar detalhes do erro** e envie o texto ao responsável pelo
Repositório Institucional do seu campus, informando o tipo de documento que estava usando.
O programa também guarda o registro em `%LOCALAPPDATA%\ExtratorRIUERN\erro.log` (Windows).
