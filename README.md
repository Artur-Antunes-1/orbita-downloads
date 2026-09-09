# Órbita — downloads

AIOS e Órbita são o mesmo projeto: um aplicativo experimental de contexto e orientação para Windows e macOS. Ele usa seu perfil, as memórias que você confirma e o contexto que autoriza para ajudar nas ferramentas compatíveis.

**[Guia das novidades e de como usar a versão 0.5](GUIA-0.5.md)**

## Baixar a versão 0.5.0

- [Windows 64 bits](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.5.0/Orbita-Windows-x64-0.5.0.zip)
- [Mac Apple Silicon — M1 ou mais novo](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.5.0/Orbita-Mac-arm64-0.5.0.zip)
- [Mac Intel](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.5.0/Orbita-Mac-x64-0.5.0.zip)
- [Hashes SHA-256](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.5.0/SHA256SUMS.txt)

Os downloads são públicos e não exigem acesso ao repositório de desenvolvimento.

## Instalação

**Windows:** extraia o ZIP inteiro para uma pasta fixa e abra `Orbita.exe`. Mantenha os arquivos juntos. `Ctrl+Shift+Espaço` abre a lateral; `Esc` recolhe.

**Mac:** requer macOS 13 ou posterior. Extraia o ZIP e arraste `Orbita.app` para Aplicativos. `Command+Shift+Espaço` abre a lateral. Autorize Acessibilidade nos ajustes do sistema para os campos compatíveis. O auxiliar nativo já vem compilado.

Abra **Painel de controle** pelo menu da Órbita ou pelo botão na lateral para usar a janela independente. Fechá-la mantém a Órbita em execução; **Sair** encerra o aplicativo.

O Windows ainda não tem assinatura comercial. O Mac usa assinatura ad hoc, sem notarização Apple. Siga o guia incluído para a exceção individual de abertura; não desative proteções globais.

## Primeiro uso

1. Complete seu perfil e configure **sua própria chave da OpenAI** em Ajustes. Confira modelo e orçamento.
2. Adicione ou importe memórias e revise as pendentes. Cada envio tem controles próprios de contexto.
3. Habilite sugestões automáticas nos aplicativos permitidos. O popup pode aparecer com o painel oculto e não envia a mensagem por você.
4. No Chrome/Edge, carregue `Extensao-Orbita` sem compactação, pareie pelo aplicativo e habilite os sites desejados. Após atualizar, recarregue a extensão e as abas. Safari não é suportado por essa extensão.
5. Para usar **Agora**, configure a conexão Google completa. Escreva uma prioridade, confira o horário proposto e aprove antes de criar o bloco. Depois do horário, relate o resultado e escolha se quer salvar uma memória pendente.

A conexão completa do Google Calendar depende de configuração OAuth e autorização da conta. iCal oferece somente leitura. O resumo e o acompanhamento locais dependem do computador ligado e da Órbita em execução. Conta/sincronização são opcionais; análises na nuvem ainda dependem de ativação do serviço.

## Dados e atualização

Os pacotes incluem aplicativo, extensão, guias genéricos e licenças. Não incluem perfil, memórias ou credenciais de outra pessoa. “Memória pública” é uma categoria de uso no aplicativo; ela não é publicada neste repositório.

Saia da Órbita antes de atualizar e extraia a nova versão em uma pasta nova. Os dados ficam separados: `%APPDATA%\Orbita` no Windows ou `~/Library/Application Support/Orbita` no Mac. Preserve essa pasta.

Os guias `GUIA-ORBITA.md`, `GUIA-MACOS.md`, `GOOGLE-CALENDAR.md`, `PRIVACIDADE.md` e `NOVIDADES-0.5.md` acompanham cada pacote. Para relatar falhas, informe versão, sistema e mensagem de erro, sem publicar chaves, tokens ou arquivos pessoais.
