# Órbita 0.5.1 — primeiro uso

A Órbita acompanha seu trabalho com contexto que você escolhe fornecer. Perfil e memória ficam neste dispositivo; enviar conteúdo à IA, sincronizar uma conta e compartilhar a agenda têm controles próprios.

**Novo na versão 0.5.1:** o acesso lateral fica recolhido em uma cápsula pequena. Passe o mouse para revelar os atalhos e clique para abrir a página desejada. Afastar o cursor recolhe os atalhos; uma página aberta por clique continua aberta. O hover não tira o foco do editor.

## Instalar e atualizar

No Windows, extraia o pacote inteiro e abra **Orbita.exe**. Mantenha os arquivos do executável juntos. No macOS, siga [GUIA-MACOS.md](GUIA-MACOS.md).

Para atualizar, saia da Órbita e substitua a pasta do aplicativo por uma extração nova. Seus dados ficam fora dela; não apague a pasta de dados durante a atualização. O pacote público contém aplicativo, extensão, guias genéricos e licenças, sem perfis, memórias ou credenciais de outra pessoa.

Os pacotes oficiais são publicados nas [versões da Órbita](https://github.com/Artur-Antunes-1/orbita-downloads/releases). Escolha a versão e a arquitetura corretas. A edição Windows ainda não tem assinatura comercial; a edição macOS usa assinatura local ad hoc, sem notarização Apple.

## Configurar seu espaço

1. Complete o perfil com atividade, objetivos, preferências e ferramentas úteis.
2. Em **Ajustes**, configure sua própria chave de IA e escolha entre os modelos disponíveis. Confira o modelo, os preços apresentados e o orçamento antes de ativar consultas automáticas. O limite local total padrão é **US$ 10**.
3. Em **Memória**, adicione ou importe fatos e revise origem, camada e projeto. Registros pendentes precisam de confirmação para participar das respostas. Por consulta, a seleção pode usar até 40 fatos elegíveis.

As camadas **Pública**, **Projeto** e **Íntima** definem situações de uso de um fato. “Pública” não significa publicação na internet. A sincronização opcional exclui fatos íntimos e registros pendentes.

## Pedir ajuda

No Windows, **Ctrl+Shift+Espaço** abre o painel e **Esc** recolhe. No Mac, use **Command+Shift+Espaço**. Os botões na borda também abrem as páginas. O menu da bandeja ou barra de menus permite pausar, ocultar e sair.

Escolha o contexto do pedido: seleção, texto copiado, captura da janela permitida ou rascunho de um editor compatível. A prévia mostra o que está disponível. Você pode retirar o contexto ou escolher quais fatos serão usados antes de enviar.

Em **Orientar**, **Revisar** ou **Escolher ferramenta**, escreva seu pedido. A resposta indica os fatos utilizados. **Copiar** deixa o texto pronto. **Aplicar no campo** depende do seu clique, confere o destino e não envia a mensagem. Quando não for possível identificar o campo com segurança, use cópia manual.

## Sugestões enquanto você escreve

Sugestões automáticas e envio automático à IA têm autorizações separadas em Ajustes. Quando habilitadas, a Órbita observa o rascunho focado de um aplicativo permitido e compatível, espera uma pausa e pode preparar uma sugestão. Capturas de tela não são incluídas automaticamente.

O popup pode aparecer com o painel recolhido e sem tirar o foco do editor. Dispensá-lo afeta aquela sugestão. **Desativar sugestões** interrompe esse comportamento; **Sair** encerra o processo. Ocultar mantém a Órbita em execução.

Se um campo não for compatível ou estiver elevado como administrador no Windows, use leitura de seleção ou **Usar texto copiado**. A lista de aplicativos permitidos e a pausa temporária ficam em Ajustes.

## Navegador

1. Em Chrome ou Edge, abra a página de extensões, habilite o modo de desenvolvedor e escolha **Carregar sem compactação**. Selecione **Extensao-Orbita**, dentro do pacote.
2. Na Órbita, habilite **Extensão do navegador**. Copie o token de pareamento em Conexões, cole no popup da extensão e confirme.
3. Ative apenas os sites desejados e recarregue as abas abertas antes da instalação.

A extensão usa o compositor focado dos sites compatíveis; não importa o histórico completo da conversa. Trocar de editor ou página invalida o contexto anterior. O token é uma credencial local: não o publique. Safari não é alvo desta extensão.

## Agenda e importações

O **Painel de controle**, aberto pela bandeja/barra de menus ou pelo botão no painel lateral, oferece uma janela independente para essas páginas e para o acompanhamento de ações. Pode ser movida, redimensionada e maximizada. Fechá-la mantém a Órbita ativa; **Voltar à lateral** recupera o modo compacto.

Na página **Agora**, informe prioridade, duração, intervalo e agenda. A Órbita verifica disponibilidade e prepara uma proposta. Revise e aprove no painel antes de criar o bloco. Depois do horário, registre seu retorno e escolha se deseja guardar algo como memória pendente. O acompanhamento fica local; o ciclo exige conexão Google completa e aplicativo em execução. Veja [NOVIDADES-0.5.md](#novidades-em-detalhe).

Em **Conexões → Google Calendar**, o endereço privado iCal permite ler a agenda real, incluindo descrições, local, organização e participantes quando fornecidos. Compartilhar disponibilidade ou detalhes com a IA é opcional.

A conexão completa por conta Google precisa da configuração OAuth do aplicativo e do seu consentimento no navegador. A interface informa quando estiver indisponível. Consulte [GOOGLE-CALENDAR.md](GOOGLE-CALENDAR.md).

Arquivos entram pelo seletor: agendas, registros de wearable, notas e cápsulas compatíveis. Você revisa os fatos importados antes de usá-los. A Órbita não varre seu disco nem interpreta dados fisiológicos como emoções.

## Conta e sincronização opcional

Em **Nuvem Órbita**, entre ou crie uma conta por e-mail e senha. Se a criação pedir confirmação de e-mail, confirme a mensagem recebida antes de entrar. Entrar não ativa automaticamente todos os compartilhamentos.

Escolha se deseja sincronizar perfil, memórias confirmadas elegíveis e feedback. O aplicativo informa o estado da conta, a sincronização e o que exige atenção. Fatos íntimos, rascunhos, capturas e detalhes transitórios da agenda ficam fora da sincronização padrão.

**Sincronizar exige login. Análises remotas exigem também configuração e liberação do operador do serviço.** Um pedido agendado não significa que uma análise foi executada. A interface informa quando o serviço não está habilitado.

## Resumos no computador

O resumo local usa a chave de IA deste dispositivo e seu controle próprio de autorização. Por padrão, tem limite de **4 análises por dia**, **US$ 0,50 por dia**, intervalo de **3 horas** e janela de **08h às 22h**, além do orçamento local total de US$ 10. Trabalha com os dados permitidos para esse recurso.

**O computador precisa estar ligado e a Órbita em execução.** Ocultar mantém o processo; encerrar o aplicativo, suspender ou desligar interrompe a execução local. Isso é independente das análises remotas do serviço.

## Dados e suporte

No Windows, os dados ficam em %APPDATA%\Orbita; no Mac, em ~/Library/Application Support/Orbita. Credenciais usam o armazenamento protegido do sistema. Exportações de memória podem conter conteúdo pessoal: revise-as antes de compartilhar.

Leia [PRIVACIDADE.md](PRIVACIDADE.md) e [NOVIDADES-0.5.md](#novidades-em-detalhe). Ao relatar um problema, envie versão, sistema e mensagem de erro. Não envie chaves, tokens, endereços privados da agenda ou sua pasta de dados.


## Novidades em detalhes

AIOS e Órbita são o mesmo projeto. Esta versão combina a presença discreta nas ferramentas com um painel independente e um primeiro ciclo de ações verificáveis.

## Popup mais rápido

A espera local foi reduzida: pausa de digitação de 400 ms no aplicativo e captura de 450 ms na extensão; nova geração pode começar a partir de cinco segundos da anterior, em vez de 30. Recapturar o mesmo texto não reinicia a espera. O pedido automático à IA foi simplificado, mantendo modelo, orçamento e validação das fontes. O tempo do provedor continua variável. Depois de atualizar a extensão, recarregue-a e recarregue as abas habilitadas.

## Painel de controle independente

Abra **Painel de controle** pelo menu da bandeja/barra de menus ou pelo botão no painel lateral. A janela pode ser movida, redimensionada e maximizada. **Voltar à lateral** recupera o acesso compacto. As janelas compartilham perfil, memória, conexões e ações. Fechar o painel maior mantém a Órbita em execução; **Sair** encerra o aplicativo. A posição e o tamanho são lembrados e recuperados quando um monitor é removido.

## Agora: da prioridade ao resultado

1. Escreva uma prioridade, escolha duração, intervalo e agenda de destino. Opcionalmente associe projeto e memórias confirmadas.
2. A Órbita consulta as agendas selecionadas e propõe um intervalo livre. Cobertura incompleta é informada; ela não é interpretada como disponibilidade.
3. Revise e aprove no painel. A criação é de um evento neutro **Bloco de foco**, sem convidados, e-mails ou lembretes padrão. A prioridade detalhada fica local.
4. A Órbita verifica o evento e guarda seu identificador. Timeout gera resultado incerto: consultar novamente não cria outro evento.
5. Depois do horário, registre se avançou, avançou parcialmente, não realizou ou adiou. Ausência de resposta permanece desconhecida.
6. Se houver algo útil para lembrar, escolha salvar para revisão. A memória nasce pendente; você decide a camada e confirma na Memória.

O horário é calculado a partir dos intervalos verificados e das reservas locais; essa proposta não exige nova chamada à IA. Evento criado comprova a operação, não a realização da tarefa nem ganho de produtividade.

**Encerrar acompanhamento** não exclui eventos no Google. Se a operação foi incerta, o evento pode existir e a reserva local é preservada. Para alterar ou excluir um evento, use os controles próprios da agenda e revise a confirmação.

## Conexão e privacidade

O ciclo exige a conexão Google completa: cliente OAuth configurado e conta autorizada para eventos e lista de agendas. iCal continua somente leitura. Configurar uma instalação não inclui suas credenciais nos instaladores públicos.

Prioridades, ações e resultados ficam neste computador e não são enviados automaticamente à Nuvem Órbita. O acompanhamento exige o aplicativo em execução; ao reabrir, operações interrompidas são verificadas sem repetir criações automaticamente. As análises remotas continuam dependendo de configuração do serviço e login e são separadas dos resumos locais e do ciclo de foco.

Veja **GUIA-ORBITA.md**, **GOOGLE-CALENDAR.md** e **PRIVACIDADE.md** no pacote. Os [downloads oficiais](https://github.com/Artur-Antunes-1/orbita-downloads/releases) contêm aplicativo, extensão, guias e licenças.



