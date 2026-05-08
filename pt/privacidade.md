# Política de Privacidade — Zplit

**Última atualização:** <<DATA_PUBLICACAO>>

> A versão em português é a juridicamente vinculante. Uma tradução em inglês está disponível em [/en/privacy](../en/privacy) para conveniência.

---

## §1 Quem somos

O Zplit (`<<NOME_FANTASIA>>`) é um aplicativo desenvolvido e operado por **<<RAZAO_SOCIAL>>**, inscrita no CNPJ sob o nº **<<CNPJ>>**, com sede em **<<CIDADE_UF>>**, Brasil. Para qualquer assunto relativo a esta Política de Privacidade ou ao tratamento dos seus dados pessoais, o canal oficial de contato é o e-mail **<<EMAIL_SUPORTE>>**.

Nos termos da **Resolução CD/ANPD nº 2/2022**, o Zplit opera como **agente de tratamento de pequeno porte**. Por essa razão, **não nomeamos um Encarregado (DPO) formal**; o canal **<<EMAIL_SUPORTE>>** é o canal oficial de comunicação com os titulares de dados e com a Autoridade Nacional de Proteção de Dados (ANPD), conforme permitido pelo regime simplificado.

## §2 O que esta política cobre

Esta Política de Privacidade descreve como tratamos seus dados pessoais quando você usa o **aplicativo Zplit** (Android, iOS e Windows) e os serviços associados, que incluem:

- O **backend hospedado no Supabase** (autenticação, banco de dados, RPCs);
- O fluxo de **importação de itens de cupom fiscal** via inteligência artificial.

Esta política aplica-se a todos os usuários do Zplit, independentemente do dispositivo ou do idioma do aplicativo.

## §3 Dados que coletamos

Coletamos somente os dados estritamente necessários para que o aplicativo funcione. Dividimos em quatro grupos:

### 3.a Dados de cadastro

- **E-mail** — usado para login, recuperação de senha e como identificador da sua conta.
- **Nome** — exibido no aplicativo e nas mensagens enviadas via WhatsApp.
- **Telefone** (opcional) — apenas se você optar por preenchê-lo no perfil.

### 3.b Dados sobre seus participantes (terceiros)

Quando você adiciona participantes a um evento, coletamos os **nomes e telefones** que você nos informa. Esses dados pertencem a terceiros (os seus participantes), e a relação jurídica é a seguinte:

- **Você é o controlador desses dados perante a LGPD.** É você quem decide quais participantes adicionar, quais dados informar e para qual finalidade.
- **O Zplit atua como operador**, processando esses dados estritamente conforme as suas instruções (armazenar, calcular divisões de despesa, gerar mensagens de cobrança via WhatsApp).
- **Você é responsável** por obter o consentimento dos participantes antes de adicioná-los, bem como por informar a eles que os dados estão sendo tratados pelo Zplit em seu nome.

Recomendamos não adicionar participantes sem que eles estejam cientes.

### 3.c Imagens de cupom fiscal

Quando você usa a função de **importar itens via cupom fiscal**, a imagem é enviada à **Google (API Gemini)** para extração automática dos itens. Importante:

- A imagem original **não é armazenada** após o processamento.
- Mantemos apenas um **registro de auditoria** (`receipt_imports`) com o status da operação (sucesso, falha, motivo da falha) por **até 30 dias**, exclusivamente para aplicar limites de uso e prevenir abuso.
- Os itens extraídos passam a fazer parte do evento como qualquer outra despesa, sob seu controle.

### 3.d O que NÃO coletamos

Para deixar claro o que está fora do escopo do Zplit:

- **Não usamos analytics de terceiros** (Google Analytics, Firebase Analytics, Mixpanel, Amplitude, etc.).
- **Não usamos redes de publicidade** (AdMob, Meta Audience, etc.).
- **Não acessamos seus contatos** do dispositivo.
- **Não coletamos dados de localização** (GPS, IP-geolocation, etc.).
- **Não coletamos dados biométricos** (face, digital, etc.).
- **Não processamos dados de pagamento** ou de cartão de crédito — o Zplit apenas calcula valores; transferências entre você e seus participantes ocorrem fora do aplicativo.

## §4 Para que usamos seus dados

Cada finalidade de tratamento está mapeada a uma base legal da **LGPD Art. 7**:

- **Permitir cadastro, login, recuperação de senha e exclusão de conta** — base legal: **execução de contrato** (Art. 7, V).
- **Salvar e exibir seus eventos, participantes, despesas e cálculos de divisão** — base legal: **execução de contrato** (Art. 7, V).
- **Importar itens via cupom fiscal** (envio à API Gemini) — base legal: **execução de contrato** — você expressamente solicitou esta operação.
- **Prevenir abuso, fraude e violações destes Termos** (limites de uso, registros de auditoria) — base legal: **legítimo interesse** (Art. 7, IX).
- **Atender a solicitações de direitos do titular** (LGPD Art. 18) — base legal: **cumprimento de obrigação legal** (Art. 7, II).

Não tratamos seus dados para nenhuma finalidade diferente das acima sem antes atualizar esta Política e informar você no aplicativo.

## §5 Com quem compartilhamos seus dados

O Zplit compartilha dados pessoais somente com os seguintes operadores nomeados, e exclusivamente nas finalidades descritas:

| Terceiro | Papel | Dados compartilhados | Política |
|---|---|---|---|
| **Supabase, Inc.** | Infraestrutura (autenticação, banco de dados, hospedagem) | Todos os dados do aplicativo (cadastro, eventos, participantes, despesas) | https://supabase.com/privacy — DPA: https://supabase.com/legal/dpa |
| **Google LLC (API Gemini)** | Processamento de imagem de cupom fiscal | Imagem enviada por você + texto extraído | https://policies.google.com/privacy |
| **WhatsApp** (Meta) | Envio de mensagem **iniciado por você** via deep link | Apenas o conteúdo da mensagem que você optar por enviar | https://www.whatsapp.com/legal/privacy-policy |

Sobre o WhatsApp: o Zplit **nunca envia mensagens em seu nome**. Quando você toca em "Enviar via WhatsApp", o Zplit apenas **abre o aplicativo de WhatsApp** instalado no seu dispositivo, com a mensagem pré-preenchida. O envio é feito pelo seu próprio aplicativo de WhatsApp, sob suas credenciais e responsabilidade.

**Não vendemos seus dados. Não compartilhamos seus dados para fins de publicidade.** Não temos parcerias comerciais nem programas de afiliados que envolvam o repasse de dados pessoais.

## §6 Onde seus dados são armazenados

Seus dados são armazenados na infraestrutura do **Supabase**, na região **<<SUPABASE_REGION>>**. Imagens de cupom fiscal, durante o processamento, são tratadas pela **Google (API Gemini)**, com infraestrutura nos **Estados Unidos**.

Como há transferência internacional de dados, adotamos como salvaguarda as **Cláusulas Contratuais Padrão (Standard Contractual Clauses)** previstas no **Data Processing Addendum (DPA) do Supabase**, em consonância com a LGPD Art. 33 (transferência internacional baseada em garantias contratuais específicas) e com as boas práticas internacionais de proteção de dados.

## §7 Por quanto tempo guardamos seus dados

- **Dados pessoais e dados dos eventos**: mantidos enquanto sua conta estiver ativa.
- **Ao excluir sua conta** (Perfil → Excluir conta): todos os dados associados (eventos, participantes, despesas, pagamentos) são apagados **imediatamente em cascata**. A operação é irreversível.
- **Registro de auditoria de cupom fiscal** (`receipt_imports`): mantido por **até 30 dias** para fins de aplicação de limites de uso e prevenção de abuso. Após esse prazo, é apagado automaticamente.
- **Backups**: a infraestrutura do Supabase mantém backups por períodos curtos para fins de continuidade do serviço; após a exclusão da conta, os dados são removidos dos backups conforme a política de retenção do Supabase.

## §8 Seus direitos como titular

Conforme a **LGPD Art. 18**, você tem os seguintes direitos sobre os seus dados pessoais:

1. **Confirmação** da existência de tratamento;
2. **Acesso** aos seus dados;
3. **Correção** de dados incompletos, inexatos ou desatualizados;
4. **Anonimização, bloqueio ou eliminação** de dados desnecessários, excessivos ou tratados em desconformidade com a LGPD;
5. **Portabilidade** dos dados a outro fornecedor;
6. **Eliminação** dos dados pessoais tratados com seu consentimento;
7. **Informação** sobre as entidades públicas e privadas com as quais o Zplit realizou uso compartilhado dos seus dados;
8. **Informação** sobre a possibilidade de não fornecer consentimento e sobre as consequências da negativa;
9. **Revogação do consentimento**, a qualquer momento.

**Como exercer:** envie um e-mail para **<<EMAIL_SUPORTE>>**. Responderemos em **até 15 dias** corridos. Para a **exclusão de conta**, você também pode usar o self-service em **Perfil → Excluir conta**, que executa a exclusão imediatamente sem necessidade de aguardar resposta.

Não há custo para o exercício dos seus direitos.

## §9 Crianças e adolescentes

O Zplit **não tem restrição etária** de acesso. Menores de 18 anos podem usar o aplicativo desde que com **consentimento e supervisão dos pais ou responsáveis legais**.

O **tratamento de dados pessoais de crianças (menores de 12 anos)** é realizado **somente com o consentimento específico e em destaque** de pelo menos um dos pais ou responsável legal, conforme **LGPD Art. 14**. Não condicionamos a participação da criança no aplicativo ao fornecimento de dados além dos estritamente necessários.

Os pais ou responsáveis podem solicitar, a qualquer momento, a **exclusão dos dados** da criança ou adolescente sob sua responsabilidade enviando e-mail para **<<EMAIL_SUPORTE>>**. A solicitação é atendida em até 15 dias.

## §10 Segurança

Adotamos medidas técnicas e administrativas adequadas ao porte da operação para proteger seus dados pessoais:

- **Comunicação por HTTPS (TLS)** em todas as requisições entre o aplicativo e o backend.
- **Criptografia em repouso** na infraestrutura do Supabase.
- **Isolamento de dados via Row Level Security (RLS)**: cada usuário só consegue acessar os próprios dados; o banco de dados é configurado para recusar acessos cruzados, mesmo em caso de bug no aplicativo.
- **Exclusão em cascata** ao remover uma conta: todos os dados associados são apagados na mesma transação.
- **Limites de uso** (rate limits) em operações sensíveis, para reduzir o risco de abuso e fraude.

Nenhum sistema é absolutamente seguro. Em caso de **incidente de segurança que possa acarretar risco ou dano relevante** aos titulares, comunicaremos a **ANPD e os titulares afetados** na forma da **LGPD Art. 48**, em prazo razoável.

## §11 Cookies, analytics e publicidade

**Atualmente, não utilizamos cookies, ferramentas de análise (analytics) de terceiros, ou redes de publicidade.** O aplicativo Zplit não integra Google Analytics, Firebase Analytics, Mixpanel, Amplitude, AdMob, Meta Audience Network, Sentry, Crashlytics, ou qualquer outra ferramenta similar.

Caso passemos a utilizar qualquer dessas tecnologias no futuro, **atualizaremos esta Política de Privacidade e notificaremos os usuários no aplicativo antes da implementação**, com tempo razoável para que você possa avaliar e, se preferir, encerrar a sua conta.

## §12 Alterações nesta política

Podemos atualizar esta Política de Privacidade de tempos em tempos para refletir mudanças na lei, em práticas operacionais ou em funcionalidades do aplicativo. A data em **"Última atualização"** (no topo do documento) sempre refletirá a versão mais recente.

Em caso de **mudanças materiais** (por exemplo, novo subprocessador, nova finalidade de tratamento, mudança na base legal), exibiremos um **aviso destacado no aplicativo** antes da entrada em vigor da nova versão, com tempo razoável para sua avaliação.

## §13 Contato

Para qualquer dúvida sobre esta Política, exercício de direitos do titular, denúncia de incidente ou qualquer outro assunto relativo a dados pessoais, entre em contato pelo e-mail:

**<<EMAIL_SUPORTE>>**

---

**Última atualização:** <<DATA_PUBLICACAO>>
