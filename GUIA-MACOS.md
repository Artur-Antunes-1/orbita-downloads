# Órbita 0.5.0 no macOS

Requer macOS 13 Ventura ou posterior. Escolha **arm64** para Apple Silicon ou **x64** para Mac Intel. O aplicativo pronto inclui o auxiliar nativo compilado; não exige Node, pnpm, Xcode ou fonte Swift para ser usado.

## Instalar

1. Baixe o pacote correspondente ao seu Mac nas [versões oficiais](https://github.com/Artur-Antunes-1/orbita-downloads/releases) e extraia o ZIP.
2. Arraste **Orbita.app** para **Aplicativos**. Mantenha **Extensao-Orbita** em um lugar fixo se for usar Chrome ou Edge.
3. Abra o aplicativo e complete o perfil. Em Ajustes, configure sua chave de IA e confira modelo e orçamento.

Esta edição tem assinatura local **ad hoc**, sem certificado de distribuição ou notarização Apple. Se o macOS bloquear um aplicativo cuja origem oficial você verificou, tente abri-lo e depois use **Ajustes do Sistema → Privacidade e Segurança → Abrir Mesmo Assim**. Confirme a exceção apenas para esse aplicativo. O procedimento é descrito pela [Apple](https://support.apple.com/pt-br/102445).

Não desative o Gatekeeper ou outras proteções globais. Se o sistema indicar malware, integridade comprometida ou aplicativo danificado, interrompa a instalação e confirme a origem e a integridade do pacote com o responsável pela distribuição.

## Permissões e uso

**Command+Shift+Espaço** abre o painel; **Esc** recolhe. O ícone da barra de menus permite abrir, ocultar, pausar e sair. Ocultar mantém o processo em execução; sair o encerra.

**Painel de controle** abre uma janela normal, movível, redimensionável e maximizável, com a página **Agora** e as páginas já existentes. Fechar essa janela mantém a Órbita na barra de menus.

Em **Ajustes → Permissões do macOS**, abra Acessibilidade, habilite a Órbita e clique em **Atualizar permissões**. Essa autorização permite ler e aplicar texto nos campos compatíveis das ferramentas permitidas. Se o sistema solicitar, encerre e reabra o aplicativo.

Captura de janela tem autorização separada e acontece quando você pede **Capturar janela**. A extensão do navegador oferece outra forma de obter o rascunho compatível, sem exigir leitura nativa por Acessibilidade.

Aplicar uma sugestão depende do seu clique, confere o campo de destino e não envia Enter. Se um editor não expuser o campo de forma compatível, copie o resultado manualmente.

## Navegador, agenda e conta

No Chrome ou Edge, carregue **Extensao-Orbita** como extensão sem compactação. Habilite a ponte em Ajustes e pareie com o token de Conexões. Ative apenas os sites desejados. A extensão não suporta Safari.

O iCal é somente leitura. A conexão completa por conta Google depende da configuração OAuth e do seu consentimento. Alterações exigem prévia e confirmação. Veja [GOOGLE-CALENDAR.md](GOOGLE-CALENDAR.md).

A sincronização opcional exige login e escolha de escopos. A criação de conta pode pedir confirmação de e-mail. Análises remotas dependem de configuração do operador. O resumo local usa sua chave de IA e só roda com o Mac ligado, acordado e a Órbita em execução.

## Atualizar e preservar dados

Encerre a Órbita antes de substituir o aplicativo. Os dados ficam em ~/Library/Application Support/Orbita, separados do pacote; não apague essa pasta ao atualizar. Credenciais usam o armazenamento protegido do macOS.

Para transferir memórias manualmente, exporte e importe uma cápsula e revise o conteúdo no destino. A cápsula pode conter dados pessoais: não a publique. Chaves e tokens não devem ser compartilhados.

## Limites desta edição

A integração nativa depende das permissões e de como cada aplicativo expõe seu editor. Compilar ou testar em um runner não substitui verificar permissões e campos no seu próprio Mac. A ausência de notarização pode exigir a exceção individual descrita acima.

As instruções completas estão em [GUIA-ORBITA.md](GUIA-ORBITA.md). O tratamento de dados está em [PRIVACIDADE.md](PRIVACIDADE.md).
