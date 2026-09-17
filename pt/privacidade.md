# Política de Privacidade — Zsplit

**Última atualização:** 17/09/2026

> A versão em português é a juridicamente vinculante. Uma tradução em inglês está disponível em [/en/privacy](../en/privacy) para conveniência.

---

## §1 Quem somos

O Zsplit é um aplicativo desenvolvido e operado por **55.936.782 LUCAS SCHMIDT**, inscrita no CNPJ sob o nº **55.936.782/0001-67**, com sede em **Blumenau/SC**, Brasil. Para qualquer assunto relativo a esta Política de Privacidade ou ao tratamento dos seus dados pessoais, o canal oficial de contato é o e-mail **zplit.team@gmail.com**.

Nos termos da **Resolução CD/ANPD nº 2/2022**, o Zsplit opera como **agente de tratamento de pequeno porte**. Por essa razão, **não nomeamos um Encarregado (DPO) formal**; o canal **zplit.team@gmail.com** é o canal oficial de comunicação com os titulares de dados e com a Autoridade Nacional de Proteção de Dados (ANPD), conforme permitido pelo regime simplificado.

## §2 O que esta política cobre

Esta Política de Privacidade descreve como tratamos seus dados pessoais quando você usa o **aplicativo Zsplit** (Android, iOS e Windows) e os serviços associados, que incluem:

- O **backend hospedado no Supabase** (autenticação, banco de dados, RPCs);
- O fluxo de **importação de itens de cupom fiscal** via inteligência artificial;
- A **compra de créditos de importação** dentro do aplicativo, pela Google Play ou pela App Store;
- O **envio de e-mails transacionais** (confirmação de cadastro, recuperação de senha e alteração de e-mail).

Esta política aplica-se a todos os usuários do Zsplit, independentemente do dispositivo ou do idioma do aplicativo.

## §3 Dados que coletamos

Coletamos somente os dados estritamente necessários para que o aplicativo funcione. Dividimos em cinco grupos:

### 3.a Dados de cadastro

- **E-mail** — usado para login, recuperação de senha e como identificador da sua conta.
- **Nome** — exibido no aplicativo e nas mensagens enviadas via WhatsApp.
- **Telefone** (opcional) — apenas se você optar por preenchê-lo no perfil.

### 3.b Dados sobre seus participantes (terceiros)

Quando você adiciona participantes a um evento, coletamos os **nomes e telefones** que você nos informa. Esses dados pertencem a terceiros (os seus participantes), e a relação jurídica é a seguinte:

- **Você é o controlador desses dados perante a LGPD.** É você quem decide quais participantes adicionar, quais dados informar e para qual finalidade.
- **O Zsplit atua como operador**, processando esses dados estritamente conforme as suas instruções (armazenar, calcular divisões de despesa, gerar mensagens de cobrança via WhatsApp).
- **Você é responsável** por obter o consentimento dos participantes antes de adicioná-los, bem como por informar a eles que os dados estão sendo tratados pelo Zsplit em seu nome.

Recomendamos não adicionar participantes sem que eles estejam cientes.

### 3.c Imagens de cupom fiscal

Quando você usa a função de **importar itens via cupom fiscal**, a imagem é enviada à **Google (API Gemini)** para extração automática dos itens. Importante:

- A imagem original **não é armazenada** após o processamento.
- Mantemos apenas um **registro de auditoria** (`receipt_imports`) com o status da operação (sucesso, falha, motivo da falha), a quantidade de itens e o valor total extraídos, e o tipo de crédito utilizado. Ele serve exclusivamente para aplicar limites de uso, prevenir abuso e estornar o crédito quando a importação falha.
- Esse registro é **apagado automaticamente 30 dias após a importação**. A única exceção é uma importação **interrompida por falha técnica** cujo crédito ainda não foi estornado: o registro é mantido até o estorno — que ocorre na próxima vez que você usar a importação — e, a partir daí, segue a regra dos 30 dias. Se isso nunca ocorrer, ele é apagado com a exclusão da sua conta.
- Os itens extraídos passam a fazer parte do evento como qualquer outra despesa, sob seu controle.

### 3.d Compras e créditos de importação

A importação via cupom fiscal consome **créditos**. Você recebe créditos gratuitos e pode comprar pacotes adicionais dentro do aplicativo. O pagamento é processado **integralmente pela Google Play** (Android) **ou pela App Store** (iOS): o Zsplit **nunca recebe** dados do seu cartão de crédito ou de outro meio de pagamento.

Para validar a compra junto à loja e creditar sua conta, mantemos:

- **Saldo de créditos** (`receipt_entitlements`) — créditos gratuitos e pagos restantes.
- **Registro de cada compra** (`receipt_purchases`) — plataforma (Android ou iOS), produto comprado, identificador e token da compra emitidos pela loja, quantidade de créditos concedida, situação da compra e data da validação.

O identificador e o token da compra são usados para confirmar a compra com a loja e para **impedir que uma mesma compra seja creditada mais de uma vez**.

### 3.e O que NÃO coletamos

Para deixar claro o que está fora do escopo do Zsplit:

- **Não usamos analytics de terceiros** (Google Analytics, Firebase Analytics, Mixpanel, Amplitude, etc.).
- **Não usamos redes de publicidade** (AdMob, Meta Audience, etc.).
- **Não acessamos seus contatos** do dispositivo.
- **Não coletamos dados de localização** (GPS, IP-geolocation, etc.).
- **Não coletamos dados biométricos** (face, digital, etc.).
- **Não recebemos dados de cartão de crédito** ou de outros meios de pagamento — compras de créditos são processadas pela Google Play ou pela App Store (ver 3.d).
- **Não intermediamos pagamentos entre você e seus participantes** — o Zsplit apenas calcula valores; as transferências ocorrem fora do aplicativo.

## §4 Para que usamos seus dados

Cada finalidade de tratamento está mapeada a uma base legal da **LGPD Art. 7**:

- **Permitir cadastro, login, recuperação de senha e exclusão de conta**, incluindo o envio dos e-mails de confirmação e de recuperação — base legal: **execução de contrato** (Art. 7, V).
- **Salvar e exibir seus eventos, participantes, despesas e cálculos de divisão** — base legal: **execução de contrato** (Art. 7, V).
- **Importar itens via cupom fiscal** (envio à API Gemini) — base legal: **execução de contrato** — você expressamente solicitou esta operação.
- **Processar compras de créditos**, validá-las junto à loja e creditar sua conta — base legal: **execução de contrato** (Art. 7, V).
- **Prevenir abuso, fraude e violações destes Termos** (limites de uso, registros de auditoria e impedir que uma mesma compra seja creditada mais de uma vez) — base legal: **legítimo interesse** (Art. 7, IX).
- **Atender a solicitações de direitos do titular** (LGPD Art. 18) — base legal: **cumprimento de obrigação legal** (Art. 7, II).

Não tratamos seus dados para nenhuma finalidade diferente das acima sem antes atualizar esta Política e informar você no aplicativo.

## §5 Com quem compartilhamos seus dados

O Zsplit compartilha dados pessoais somente com os seguintes operadores nomeados, e exclusivamente nas finalidades descritas:

| Terceiro | Papel | Dados compartilhados | Política |
|---|---|---|---|
| **Supabase, Inc.** | Infraestrutura (autenticação, banco de dados, hospedagem) | Todos os dados do aplicativo (cadastro, eventos, participantes, despesas, créditos e compras) | https://supabase.com/privacy — DPA: https://supabase.com/legal/customer-resources/data-processing-addendum |
| **Google LLC (API Gemini)** | Processamento de imagem de cupom fiscal | Imagem enviada por você + texto extraído | https://policies.google.com/privacy |
| **Resend, Inc.** | Envio de e-mails transacionais (confirmação de cadastro, recuperação de senha e alteração de e-mail) | Seu endereço de e-mail e o conteúdo da mensagem | https://resend.com/legal/privacy-policy — DPA: https://resend.com/legal/dpa |
| **Google LLC (Google Play)** | Processamento do pagamento e validação de compras no Android | Identificador do produto e token da compra, para confirmar que a compra é válida | https://policies.google.com/privacy |
| **Apple Inc. (App Store)** | Processamento do pagamento e validação de compras no iOS | Identificador da transação, para confirmar que a compra é válida | https://www.apple.com/legal/privacy/ |
| **WhatsApp** (Meta) | Envio de mensagem **iniciado por você** via deep link | Apenas o conteúdo da mensagem que você optar por enviar | https://www.whatsapp.com/legal/privacy-policy |

Sobre as lojas: a compra é realizada **diretamente entre você e a Google Play ou a App Store**, que tratam os dados de pagamento conforme as próprias políticas. O Zsplit apenas consulta a loja para confirmar que a compra é válida antes de creditar sua conta.

Sobre o WhatsApp: o Zsplit **nunca envia mensagens em seu nome**. Quando você toca em "Enviar via WhatsApp", o Zsplit apenas **abre o aplicativo de WhatsApp** instalado no seu dispositivo, com a mensagem pré-preenchida. O envio é feito pelo seu próprio aplicativo de WhatsApp, sob suas credenciais e responsabilidade.

**Não vendemos seus dados. Não compartilhamos seus dados para fins de publicidade.** Não temos parcerias comerciais nem programas de afiliados que envolvam o repasse de dados pessoais.

## §6 Onde seus dados são armazenados

Seus dados são armazenados na infraestrutura do **Supabase**, na região **us-east-1**. Imagens de cupom fiscal, durante o processamento, são tratadas pela **Google (API Gemini)**, com infraestrutura nos **Estados Unidos**. E-mails transacionais são enviados pela **Resend, Inc.**, empresa sediada nos **Estados Unidos**, com a infraestrutura de envio configurada na região de **São Paulo (sa-east-1)**.

Como há transferência internacional de dados, adotamos como salvaguarda as garantias contratuais previstas nos **Data Processing Addendums (DPA)** do Supabase e da Resend — no caso do Supabase, as **Cláusulas Contratuais Padrão (Standard Contractual Clauses)** —, em consonância com a LGPD Art. 33 (transferência internacional baseada em garantias contratuais específicas) e com as boas práticas internacionais de proteção de dados.

## §7 Por quanto tempo guardamos seus dados

- **Dados pessoais e dados dos eventos**: mantidos enquanto sua conta estiver ativa.
- **Ao excluir sua conta** (Perfil → Excluir conta): todos os dados associados (eventos, participantes, despesas, pagamentos entre participantes, saldo de créditos, registros de compra e registros de importação) são apagados **imediatamente em cascata**. A operação é irreversível.
- **Registro de auditoria de cupom fiscal** (`receipt_imports`): **apagado automaticamente 30 dias após a importação**, por uma rotina diária. Exceção: o registro de uma importação interrompida por falha técnica, cujo crédito ainda não foi estornado, é mantido até o estorno (ver 3.c).
- **Saldo de créditos e registros de compra** (`receipt_entitlements`, `receipt_purchases`): mantidos enquanto sua conta estiver ativa e apagados com a exclusão da conta. A Google Play e a App Store mantêm os próprios registros da transação, conforme as políticas delas — a exclusão da sua conta no Zsplit não os apaga.
- **Backups**: a infraestrutura do Supabase mantém backups por períodos curtos para fins de continuidade do serviço; após a exclusão da conta, os dados são removidos dos backups conforme a política de retenção do Supabase.

## §8 Seus direitos como titular

Conforme a **LGPD Art. 18**, você tem os seguintes direitos sobre os seus dados pessoais:

1. **Confirmação** da existência de tratamento;
2. **Acesso** aos seus dados;
3. **Correção** de dados incompletos, inexatos ou desatualizados;
4. **Anonimização, bloqueio ou eliminação** de dados desnecessários, excessivos ou tratados em desconformidade com a LGPD;
5. **Portabilidade** dos dados a outro fornecedor;
6. **Eliminação** dos dados pessoais tratados com seu consentimento;
7. **Informação** sobre as entidades públicas e privadas com as quais o Zsplit realizou uso compartilhado dos seus dados;
8. **Informação** sobre a possibilidade de não fornecer consentimento e sobre as consequências da negativa;
9. **Revogação do consentimento**, a qualquer momento.

**Como exercer:** envie um e-mail para **zplit.team@gmail.com**. Responderemos em **até 15 dias** corridos. Para a **exclusão de conta**, você também pode usar o self-service em **Perfil → Excluir conta**, que executa a exclusão imediatamente sem necessidade de aguardar resposta.

Não há custo para o exercício dos seus direitos.

## §9 Crianças e adolescentes

O Zsplit **não tem restrição etária** de acesso. Menores de 18 anos podem usar o aplicativo desde que com **consentimento e supervisão dos pais ou responsáveis legais**.

O **tratamento de dados pessoais de crianças (menores de 12 anos)** é realizado **somente com o consentimento específico e em destaque** de pelo menos um dos pais ou responsável legal, conforme **LGPD Art. 14**. Não condicionamos a participação da criança no aplicativo ao fornecimento de dados além dos estritamente necessários.

Os pais ou responsáveis podem solicitar, a qualquer momento, a **exclusão dos dados** da criança ou adolescente sob sua responsabilidade enviando e-mail para **zplit.team@gmail.com**. A solicitação é atendida em até 15 dias.

## §10 Segurança

Adotamos medidas técnicas e administrativas adequadas ao porte da operação para proteger seus dados pessoais:

- **Comunicação por HTTPS (TLS)** em todas as requisições entre o aplicativo e o backend.
- **Criptografia em repouso** na infraestrutura do Supabase.
- **Isolamento de dados via Row Level Security (RLS)**: cada usuário só consegue acessar os próprios dados; o banco de dados é configurado para recusar acessos cruzados, mesmo em caso de bug no aplicativo.
- **Exclusão em cascata** ao remover uma conta: todos os dados associados são apagados na mesma transação.
- **Limites de uso** (rate limits) em operações sensíveis, para reduzir o risco de abuso e fraude.

Nenhum sistema é absolutamente seguro. Em caso de **incidente de segurança que possa acarretar risco ou dano relevante** aos titulares, comunicaremos a **ANPD e os titulares afetados** na forma da **LGPD Art. 48**, em prazo razoável.

## §11 Cookies, analytics e publicidade

**Atualmente, não utilizamos cookies, ferramentas de análise (analytics) de terceiros, ou redes de publicidade.** O aplicativo Zsplit não integra Google Analytics, Firebase Analytics, Mixpanel, Amplitude, AdMob, Meta Audience Network, Sentry, Crashlytics, ou qualquer outra ferramenta similar.

Caso passemos a utilizar qualquer dessas tecnologias no futuro, **atualizaremos esta Política de Privacidade e notificaremos os usuários no aplicativo antes da implementação**, com tempo razoável para que você possa avaliar e, se preferir, encerrar a sua conta.

## §12 Alterações nesta política

Podemos atualizar esta Política de Privacidade de tempos em tempos para refletir mudanças na lei, em práticas operacionais ou em funcionalidades do aplicativo. A data em **"Última atualização"** (no topo do documento) sempre refletirá a versão mais recente.

Em caso de **mudanças materiais** (por exemplo, novo subprocessador, nova finalidade de tratamento, mudança na base legal), exibiremos um **aviso destacado no aplicativo** antes da entrada em vigor da nova versão, com tempo razoável para sua avaliação.

## §13 Contato

Para qualquer dúvida sobre esta Política, exercício de direitos do titular, denúncia de incidente ou qualquer outro assunto relativo a dados pessoais, entre em contato pelo e-mail:

**zplit.team@gmail.com**

---

**Última atualização:** 17/09/2026
