# Privacidade na Órbita 0.5.0

Contexto local, consultas de IA, sugestões automáticas, agenda e sincronização têm controles separados. Conectar uma fonte ou criar uma conta não autoriza todos os usos dos seus dados.

## No dispositivo

Perfil, memórias, preferências e registros operacionais ficam na pasta de dados: %APPDATA%\Orbita no Windows ou ~/Library/Application Support/Orbita no macOS. Ela é separada do pacote distribuído.

Chaves de IA, tokens de conta e pareamento e endereços privados da agenda usam o armazenamento protegido do sistema via Electron safeStorage. Essa proteção não isola a conta do computador de outros programas executados pelo mesmo usuário. Não compartilhe credenciais ou sua pasta de dados.

Exportações de memória são arquivos que você decide criar e podem conter conteúdo pessoal. Revise antes de compartilhar. Os pacotes públicos não incluem uma exportação de usuário.

## Envio à IA

Uma consulta pode incluir seu pedido, perfil pertinente, fatos elegíveis escolhidos e o contexto que você decidiu incluir. O provedor configurado recebe o necessário para responder. Custos e tratamento no provedor seguem a conta e as condições desse serviço.

Leitura de seleção, texto copiado e captura dependem do seu gesto. Rascunhos de aplicativos permitidos podem ser observados com sugestões automáticas ativas. O envio automático à IA tem controle próprio; capturas não são enviadas automaticamente por esse fluxo.

Capturas e contextos completos são transitórios. Orientações da sessão podem depender de fatos e permissões usados no pedido; remover a fonte ou revogar a autorização impede sua reutilização em consultas posteriores. O diário opcional registra eventos e custos sem arquivar o texto completo de cada consulta.

Fatos íntimos seguem suas regras de contexto local. “Pública” é uma camada de uso, não publicação na internet. Registros pendentes não se tornam confirmados sem revisão.

## Google Calendar

Ler a agenda não ativa o envio de detalhes à IA. Disponibilidade livre/ocupado e contexto completo têm autorizações independentes. O contexto completo tem limite, origem, cobertura e expiração.

Descrições e participantes não são automaticamente promovidos a memória pública e ficam fora da sincronização padrão. O cache iCal é mínimo; endereço e tokens ficam protegidos separadamente. A conexão OAuth solicita revogação ao desconectar. Veja [GOOGLE-CALENDAR.md](GOOGLE-CALENDAR.md).

Criar, editar ou excluir exige confirmação de uma prévia. E-mails de atualização dependem da escolha no editor e do comportamento documentado pelo Google.

## Nuvem Órbita

Sincronização exige login e consentimento para os escopos escolhidos. Dados são associados à sua conta e têm regras de acesso por usuário. Isso não é criptografia de ponta a ponta: o serviço processa os dados autorizados para sincronizar e oferecer análises habilitadas.

Os escopos incluem perfil, memórias confirmadas elegíveis das camadas permitidas e feedback. Fatos íntimos, registros pendentes, credenciais, rascunhos, capturas e detalhes transitórios da agenda ficam fora da sincronização padrão. Alterar os escopos modifica o conjunto autorizado.

Análises remotas precisam de autorização da conta e configuração do operador. A opção não garante execução quando o serviço está desativado. A interface informa o estado. A chave de IA do computador não é enviada como credencial ao trabalhador remoto.

Sair da conta encerra a sessão local; não equivale a apagar os dados remotos. Use o controle de exclusão remota e confirme o resultado apresentado. A cópia local e exportações que você já criou têm controles próprios.

## Resumos locais e aplicação de texto

O ciclo de foco guarda localmente prioridade, proposta, aprovação, identificação do evento e retorno declarado pelo usuário. Esses registros não entram automaticamente na projeção da nuvem. O evento criado usa título neutro e não recebe a prioridade detalhada, convidados ou lembretes padrão. Encerrar acompanhamento não exclui o evento. Salvar um resultado como memória é uma ação separada e produz um registro pendente para revisão.

O resumo local tem autorização própria e usa os dados permitidos com a chave de IA deste computador. Respeita limites de frequência, gasto e orçamento total. Só roda com o computador ligado e a Órbita em execução, independentemente das análises remotas.

Aplicar texto exige seu clique e não envia a mensagem. A extensão usa o compositor compatível em foco, sem importar o histórico completo. Você pode desabilitar aplicativos, sites, sugestões e a ponte do navegador.

## Revisar ou interromper

- Revise, edite ou exclua fatos na Memória.
- Retire contexto de uma consulta ou desligue sugestões e envio automático à IA.
- Desative o compartilhamento da agenda ou desconecte a fonte.
- Revise escopos da conta, saia da nuvem ou use exclusão remota.
- Encerre a Órbita para interromper o processamento local em segundo plano.

Para suporte, compartilhe versão, sistema e mensagem de erro. Evite capturas com dados pessoais e nunca envie chaves, tokens ou endereço secreto iCal.
