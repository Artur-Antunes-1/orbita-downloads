# Órbita 0.4 — guia das novidades

Este guia reúne as novidades e os principais recursos da versão 0.4.0, com os caminhos reais dentro do aplicativo. Publicado em 09/09/2026.

## Downloads públicos

Compartilhe a [página de download](https://github.com/Artur-Antunes-1/orbita-downloads/releases/tag/v0.4.0). Ela não exige acesso ao repositório privado nem login no GitHub.

| Sistema | Arquivo |
| --- | --- |
| Windows 64 bits | [Baixar Windows x64](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Windows-x64-0.4.0.zip) |
| Mac com M1 ou posterior | [Baixar Mac Apple Silicon](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Mac-arm64-0.4.0.zip) |
| Mac Intel | [Baixar Mac Intel](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/Orbita-Mac-x64-0.4.0.zip) |

O pacote inclui aplicativo, extensão Chrome/Edge, guias e licenças. Cada pessoa configura seu próprio perfil e chave de IA; nenhum dado pessoal de outra pessoa acompanha o download. Os [hashes SHA-256](https://github.com/Artur-Antunes-1/orbita-downloads/releases/download/v0.4.0/SHA256SUMS.txt) permitem conferir os arquivos.

## Instalar e começar

**Windows:** extraia o ZIP inteiro para uma pasta fixa e abra **Orbita.exe**. Mantenha os demais arquivos junto dele. **Ctrl+Shift+Espaço** abre o painel; **Esc** recolhe.

**Mac:** requer macOS 13 ou posterior. Extraia o ZIP, mova **Orbita.app** para Aplicativos e abra. **Command+Shift+Espaço** abre o painel. Em **Ajustes → Permissões do macOS**, autorize Acessibilidade e atualize as permissões para usar os campos compatíveis.

O Mac ainda usa assinatura ad hoc, sem notarização Apple. Se houver bloqueio por desenvolvedor não identificado, verifique a origem e siga a exceção individual descrita pela [Apple](https://support.apple.com/pt-br/102445). Não desative as proteções globais. O Windows ainda não tem assinatura comercial.

Para quem já usa a Órbita: saia pelo menu da bandeja/barra de menus antes de substituir os arquivos. O perfil e as memórias ficam fora da pasta do aplicativo e devem ser preservados.

No primeiro uso, complete o perfil. Depois, abra **Ajustes → Inteligência**, configure **Chave de API OpenAI → Salvar chave** e confira **Modelo** e orçamento. O seletor oferece **GPT-5.6 Luna** e **GPT-5.4 mini**. O modelo escolhido vale para as consultas seguintes. O limite total local padrão é US$ 10; os resumos também consomem esse orçamento.

## 1. Popup com o painel oculto

A Órbita pode preparar uma melhoria do rascunho e mostrar um popup independente, sem exigir que o painel principal esteja aberto. Ela precisa continuar em execução na bandeja ou na barra de menus.

1. Em **Ajustes**, confira se sugestões automáticas, envio automático à IA e leitura passiva estão habilitados, sem pausa ativa.
2. Use um campo de prompt compatível em um aplicativo permitido e escreva um pedido completo.
3. Pare de digitar por alguns instantes. A Órbita verifica se há uma sugestão aplicável; pedidos muito curtos, repetidos ou sem mudança útil podem não gerar popup.
4. Compare **Original** e **Sugestão**. Abra **Por que esta sugestão** para entender o contexto utilizado.
5. Escolha **Aplicar no campo** ou **Copiar**. Aplicar depende do seu clique e não envia a mensagem nem pressiona Enter.

Exemplo para testar:

> Crie um formulário de cadastro em React com campos de nome e e-mail, mensagens de validação claras e navegação por teclado.

Fechar uma sugestão dispensa aquela intervenção. **Desativar sugestões** interrompe as sugestões automáticas. **Sair** encerra o aplicativo; ocultar o painel mantém o processo ativo. Capturas de tela continuam sob demanda.

**No navegador:** carregue **Extensao-Orbita** em Chrome ou Edge como extensão sem compactação. Habilite a ponte no aplicativo, copie o token em Conexões e pareie pela extensão. Ative os sites desejados e recarregue as abas. A extensão acompanha o compositor compatível em foco; não importa o histórico completo da conversa. Safari não é suportado nesta versão.

## 2. Contexto automático por projeto

Em **Orientação → Projeto**, deixe **Detectar pelo contexto** ou escolha um projeto existente.

No modo **Automática**, a Órbita seleciona memórias confirmadas relevantes para o pedido e o projeto. Abra a contagem de fatos para ver **Contexto que será usado**. Cada fato mostra sua origem e pode ser retirado daquela consulta.

No modo **Manual**, escolha os fatos que deseja incluir. Selecionar nenhum mantém a consulta sem memórias selecionadas; seu perfil informado continua sendo considerado.

Seleção, texto copiado, captura de janela e rascunho do editor continuam sendo fontes separadas. Confira a opção de incluir o contexto antes de enviar. Memórias pendentes não entram nas respostas, e fatos íntimos ficam fora da seleção automática e da sincronização.

Exemplo: escolha o projeto em que está trabalhando e peça “Qual deve ser meu próximo passo?”. Confira a prévia para saber quais fatos sustentam a orientação.

## 3. Continuar uma orientação

Você pode enviar outro pedido na conversa atual, como “Transforme isso em três passos” ou “Detalhe apenas o primeiro passo”. Não é preciso copiar a resposta anterior para explicar tudo novamente.

**Ver histórico** permite abrir respostas da sessão; use **Continuar conversa** quando a ação estiver disponível. **Nova conversa** reinicia o contexto da conversa.

Essa continuidade é temporária, durante a sessão do aplicativo, e mantém até seis rodadas. Ela não é um arquivo permanente de todas as conversas. Alterar ou retirar uma fonte pode invalidar o histórico que dependia dela.

## 4. Revisar memórias em grupo

Abra **Memória → Revisar**. Os registros pendentes ficam agrupados para facilitar a leitura da origem.

Você pode marcar registros individualmente ou usar **Selecionar N visíveis**. Depois de conferir os fatos, use **Confirmar N**. Edite ou exclua o que estiver incorreto; importar um arquivo não confirma automaticamente seu conteúdo.

Uma importação de arquivo também não equivale a uma conexão contínua com o serviço de origem. Novos dados só chegarão por uma nova importação ou por um conector realmente configurado.

As camadas **Pública**, **Projeto** e **Íntima** organizam o uso dos fatos. “Pública” não significa publicação na internet. Nenhuma memória pessoal é publicada no repositório de downloads.

## 5. Feedback sobre a ajuda

Abaixo da resposta, use **Esta orientação ajudou? → Sim / Não**. O popup também oferece **Sim / Não**.

O aplicativo registra esse retorno para revisão e, se autorizado, sincronização. Isso não significa que ele já tenha um sistema comprovado de aprendizado personalizado a partir de cada clique, nem que o feedback autorize novas ações.

## 6. Seu resumo automático local

Na parte inferior de **Orientação**, encontre **Seu resumo** e habilite **Preparar resumos automaticamente**. **Preparar agora** solicita um resumo; após existir um resultado, o botão passa a ser **Atualizar**.

O resumo usa seu perfil e até 12 memórias confirmadas públicas ou de projeto, com a chave de IA dos Ajustes. Mostra o texto, os próximos passos, a contagem de fontes usadas e o modelo. Dados íntimos, rascunhos, capturas e histórico de conversa não alimentam esse recurso.

Os automáticos funcionam entre **8h e 22h no horário de Fortaleza**, com intervalo mínimo de **três horas**, até **quatro tentativas** e **US$ 0,50 por dia**, dentro do orçamento local total. Conteúdo igual pode ser reaproveitado; esses limites não significam que quatro resumos serão gerados todos os dias. A solicitação manual também respeita os limites de tentativas e custo.

**O computador precisa estar acordado e a Órbita em execução.** O cartão identifica o resultado como preparado neste computador. Desligar o recurso interrompe novos resumos e retira o resultado; pausar a Órbita impede novos envios em segundo plano.

## 7. Google Calendar com mais contexto

**Disponível por iCal, somente leitura:** títulos, horários, descrição, local, organização e participantes, quando fornecidos pelo Google.

Para conectar, no Google Calendar abra as configurações da agenda, entre em **Integrar agenda** e copie o **Endereço secreto no formato iCal**. Esse caminho é descrito na [ajuda oficial do Google](https://support.google.com/calendar/answer/37648?hl=pt-BR). Mantenha esse endereço privado.

Na Órbita, abra **Conexões → Google Calendar → Agenda por endereço privado**, cole em **Endereço privado iCal** e use **Conectar endereço**.

Existem duas autorizações independentes:

| Controle | O que compartilha |
| --- | --- |
| Compartilhar apenas minha disponibilidade | Resumo temporário de livre/ocupado, sem títulos, descrições ou participantes. |
| Usar detalhes da agenda nas respostas da IA | Eventos e detalhes relevantes ao pedir orientação com contexto. |

O contexto completo enviado à IA é limitado a dez eventos dos próximos 14 dias e pode ser parcial. Ele expira e não se transforma automaticamente em memória pública. Um erro de atualização não é interpretado como agenda livre; dados em cache são identificados como precisando de atualização.

**Ainda depende de configuração:** entrar com a conta Google e criar, editar ou excluir eventos. O fluxo foi implementado, mas a edição distribuída precisa da configuração OAuth e da autorização da conta. Quando disponível, cada alteração exige prévia e confirmação; iCal nunca permite editar eventos.

## 8. Conta e Nuvem Órbita

Abra **Conexões → Nuvem Órbita → Entrar / Criar conta**. A conta usa e-mail e senha e pode exigir confirmação de e-mail.

Os escopos disponíveis são **Perfil**, **Memórias confirmadas**, **Feedback** e **Análise em segundo plano**. **Autorizar e sincronizar** inicia a sincronização escolhida; depois há **Salvar permissões** e **Sincronizar agora**.

Na entrega 0.4, a base está publicada, mas o fluxo completo ainda precisa de validação com conta real. **As análises remotas ainda não estão ativadas pelo serviço.** Criar uma conta ou marcar análise em segundo plano não faz um agente começar a processar dados na nuvem. Use o resumo local enquanto essa configuração não for concluída.

A sincronização exclui memórias íntimas e pendentes, rascunhos, capturas, áudios e detalhes transitórios da agenda. Sair da conta encerra a sessão local; para apagar a cópia remota, use o controle próprio de exclusão e confira o resultado. Uma instalação envia o contexto principal; as demais não substituem esse conjunto automaticamente.

## 9. Design e confiabilidade

O visual escuro e lavanda foi preservado. A versão melhora a adaptação a janelas menores, foco do teclado, transições, carregamento, textos longos e estados de erro. Também respeita a preferência por movimento reduzido do sistema.

A gravação de dados ganhou tratamento para bloqueios transitórios de arquivos no Windows. Uma falha persistente mantém a proteção do orçamento. As consultas também revalidam as fontes antes de usar ou mostrar um resultado.

## 10. Diagnóstico e problemas comuns

Em **Ajustes → Diagnóstico**, use **Copiar diagnóstico seguro** para obter informações de versão, estado e contagens. Ele não inclui sua chave, token de pareamento ou texto bruto de contexto.

| Situação | O que conferir |
| --- | --- |
| O popup não aparece | Aplicativo em execução, perfil completo, chave válida, orçamento disponível, sugestões/envio automático/leitura passiva habilitados, ausência de pausa e campo permitido em foco. |
| Não funciona no navegador | Extensão carregada, pareamento concluído, ponte habilitada, site autorizado e aba recarregada. |
| Não consegue ler ou aplicar no Windows | Confirme que a sessão está interativa e o editor expõe um campo compatível. Para campos elevados como administrador ou incompatíveis, use copiar/colar manual. |
| Não consegue ler ou aplicar no Mac | Confira Acessibilidade em Ajustes do Sistema e atualize as permissões no aplicativo. |
| Não aparece resumo novo | Confira se o recurso está ativo, se há contexto confirmado, se o computador está acordado e se intervalo/orçamento permitem nova tentativa. |
| A nuvem não gera análise | A ativação remota ainda está pendente na entrega 0.4; o resumo local é um recurso separado. |
| A agenda não permite editar | iCal é somente leitura; edição depende da conexão Google completa e de permissão na agenda. |

Os testes automatizados e de interface passaram. A interação nativa foi validada no runner Mac; a repetição atual de foco/aplicação no Windows ficou bloqueada pela ausência de uma sessão desktop interativa. A compatibilidade de cada campo ainda deve ser confirmada no computador usado para o teste.

## Um roteiro de cinco minutos

1. Abra a Órbita e confira perfil, modelo e chave.
2. Revise algumas memórias pendentes e confirme as corretas.
3. Em Orientação, escolha um projeto, veja a prévia dos fatos e peça um próximo passo.
4. Continue a conversa e dê feedback sobre a resposta.
5. Confira **Seu resumo**, oculte o painel e teste um rascunho completo no aplicativo ou site permitido.

Os guias de primeiro uso, macOS, Google Calendar e privacidade também acompanham o ZIP.
