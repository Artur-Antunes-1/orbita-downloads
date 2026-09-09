# Órbita — downloads

Órbita é um aplicativo experimental de contexto e orientação para Windows e macOS. Ele usa seu perfil, as memórias que você confirma e o contexto que autoriza para ajudar nos aplicativos compatíveis.

## Baixar a versão 0.4.0

- [Windows 64 bits](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Windows-x64-0.4.0.zip)
- [Mac Apple Silicon — M1, M2, M3 e posteriores](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Mac-arm64-0.4.0.zip)
- [Mac Intel](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Mac-x64-0.4.0.zip)
- [Hashes SHA-256](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/SHA256SUMS.txt)

Os downloads são públicos e não exigem acesso ao repositório de desenvolvimento.

## Instalação

**Windows:** extraia o ZIP inteiro para uma pasta fixa e abra `Orbita.exe`. O aplicativo depende dos outros arquivos da pasta. `Ctrl+Shift+Espaço` abre o painel; `Esc` recolhe.

**Mac:** requer macOS 13 ou posterior. Extraia o ZIP e arraste `Orbita.app` para Aplicativos. `Command+Shift+Espaço` abre o painel. Autorize Acessibilidade nos ajustes do sistema para os campos compatíveis. O pacote já inclui o auxiliar nativo compilado.

O Windows ainda não tem assinatura comercial. O Mac usa assinatura ad hoc, sem notarização Apple; siga o guia incluído e, quando aplicável, use a exceção individual em Privacidade e Segurança. Não desative proteções globais do sistema.

## Primeiro uso

1. Complete seu perfil e configure **sua própria chave da OpenAI** em Ajustes. Confira modelo e orçamento.
2. Adicione ou importe memórias e revise as pendentes. Cada envio tem controles próprios de contexto.
3. Habilite sugestões automáticas nos aplicativos permitidos. O popup pode aparecer com o painel oculto, sem enviar o texto por você. O processo da Órbita precisa continuar em execução.
4. Para Chrome/Edge, carregue a pasta `Extensao-Orbita` como extensão sem compactação, pareie com o token mostrado no aplicativo e habilite os sites desejados. Safari não é suportado nesta versão.

O resumo local funciona com o computador acordado e a Órbita em execução. A conexão completa do Google Calendar depende de configuração OAuth; o endereço privado iCal oferece leitura. Conta/sincronização são opcionais; análises na nuvem dependem de ativação do serviço e ainda não estão operacionais nesta edição.

## Dados e atualização

Os pacotes incluem apenas aplicativo, extensão, guias genéricos e licenças. Não incluem perfil, memórias ou credenciais de outra pessoa. “Memória pública” é uma categoria de uso no aplicativo; ela não é publicada neste repositório.

Saia da Órbita antes de atualizar e extraia a nova versão em uma pasta nova. Os dados ficam separados: `%APPDATA%\Orbita` no Windows ou `~/Library/Application Support/Orbita` no Mac. Preserve essa pasta.

Os guias `GUIA-ORBITA.md`, `GUIA-MACOS.md`, `GOOGLE-CALENDAR.md` e `PRIVACIDADE.md` acompanham cada pacote. Para relatar falhas, informe versão, sistema e mensagem de erro; não publique chaves, tokens, arquivos pessoais ou endereços privados da agenda.
