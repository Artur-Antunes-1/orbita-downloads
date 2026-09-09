# Google Calendar na Órbita 0.5.0

A Órbita oferece leitura por endereço privado iCal e conexão completa por conta Google. A interface informa o que está disponível e quais permissões foram concedidas.

## Ler uma agenda por iCal

1. No Google Calendar, abra **Configurações**, escolha uma agenda e entre em **Integrar agenda**.
2. Copie o **Endereço secreto no formato iCal**.
3. Na Órbita, abra **Conexões → Google Calendar → Agenda por endereço privado**.
4. Cole no campo **Endereço privado iCal** e clique em **Conectar endereço**.

Esse endereço permite ler a agenda e deve ficar restrito a você. Se for exposto, redefina-o no Google e conecte o novo valor. Contas de trabalho ou estudo podem não oferecer essa opção. Consulte a [orientação oficial do Google](https://support.google.com/calendar/answer/37648?hl=pt-BR).

O iCal é **somente leitura**. Mostra títulos, horários, descrições, local, organização e participantes quando fornecidos. A consulta ocorre ao conectar, ao abrir a Órbita e a cada cinco minutos enquanto ela estiver em execução, além da atualização manual. O feed pode ter atraso do próprio Google.

## Conectar a conta Google

Quando disponível, **Conectar conta Google** abre a autorização no navegador do sistema. Você escolhe a conta e as permissões. A Órbita não extrai cookies, senhas ou sessões de outros aplicativos.

A edição 0.5.0 inclui autorização e edição, mas depende de um cliente OAuth Desktop configurado pelo responsável pela distribuição. Se a interface informar que aguarda configuração, o botão não representa uma conta conectada. O iCal continua disponível. A conexão real só existe depois do consentimento no Google e da leitura bem-sucedida.

Eventos e lista de agendas têm permissões separadas. Recusar uma parte mantém as limitações visíveis. Agendas compartilhadas somente para leitura continuam sem edição.

## Criar, editar e excluir

Com conta autorizada e agenda editável, use **Criar evento** ou abra um evento e escolha **Editar ou excluir evento**. Informe título, datas, descrição, local e participantes necessários.

A prévia mostra o estado anterior, o resultado proposto, a agenda de destino e as notificações escolhidas. **Confirmar** envia a operação ao Google; a IA não executa essas ações autonomamente.

- A prévia vale por dois minutos e pode ser usada uma vez.
- Se o evento mudar no Google, atualize a agenda e prepare outra prévia. A versão antiga não é sobrescrita silenciosamente.
- Campos não alterados são preservados. Textos ou participantes incompletos por excederem o limite local devem ser editados no Google Calendar.
- Em recorrências, a edição vale para a ocorrência selecionada. A série inteira e certos tipos especiais ficam fora da edição local.
- Em eventos de dia inteiro, a data final é exclusiva: para um único dia, escolha como fim o dia seguinte.

O padrão é **não solicitar envio de e-mails**. Você pode escolher todos os participantes ou somente participantes externos ao Google Calendar. O Google informa que alguns avisos ainda podem ser enviados; suprimir atualizações pode afetar a sincronização de convidados externos. Veja a [documentação de atualização de eventos](https://developers.google.com/workspace/calendar/api/v3/reference/events/patch).

## Escolher o uso pela IA

Os controles são independentes e começam desligados:

| Controle | Autoriza |
| --- | --- |
| Compartilhar apenas minha disponibilidade | Resumo temporário de livre/ocupado da agenda iCal, sem títulos, descrições ou participantes. |
| Usar detalhes da agenda nas respostas da IA | Enviar eventos relevantes e detalhes disponíveis ao provedor de IA configurado ao pedir ajuda com contexto. |

O contexto completo inclui até **10 eventos** relevantes dos próximos **14 dias**, com limite de **20 KB em UTF-8** para dados e metadados e validade de cinco minutos. A cobertura indica conteúdo adicional não incluído. Falhas de leitura não são interpretadas como agenda livre.

Detalhes são tratados como dados externos, não como instruções. Não viram automaticamente memória pública nem entram na sincronização padrão da Nuvem Órbita. Você pode desligar esse uso e continuar consultando a agenda local.

## Dados locais e desconexão

A interface lista até 100 eventos dos próximos 14 dias, incluindo os em andamento. A conta consulta até 30 agendas por leitura; a cobertura parcial é informada. Textos e participantes têm limites de exibição.

O endereço privado e os tokens OAuth ficam no armazenamento protegido e não voltam à interface. O cache iCal guarda títulos e horários; descrições e participantes completos ficam na sessão local. O módulo de API não grava uma cópia dos eventos completos em disco.

**Desconectar endereço** remove a URL protegida, o cache e os eventos locais do feed. **Desconectar conta** remove os tokens locais e solicita revogação no Google. Falhas de rede nessa revogação são informadas; revise o acesso nas configurações da conta se necessário. Desconectar não exclui eventos no Google.

Leia também [PRIVACIDADE.md](PRIVACIDADE.md).
