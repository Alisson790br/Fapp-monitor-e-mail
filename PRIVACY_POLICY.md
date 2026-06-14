# Política de Privacidade

**Extensão FAPP — Monitor & E-mail (Dynamics)** · Atualizada em 14/06/2026

Esta extensão foi criada para apoiar o atendimento ao cliente (CX) sobre ocorrências do Microsoft Dynamics 365. Esta política explica, de forma clara, quais dados a extensão acessa, como eles são tratados e quais nunca saem do seu navegador.

## 1. Princípio geral
A extensão funciona **inteiramente dentro do seu navegador e da sua sessão já autenticada no Dynamics 365**. Ela **não envia nenhum dado para servidores externos, terceiros ou para o desenvolvedor**. Não há analytics, rastreamento, anúncios nem coleta de dados para fins comerciais.

## 2. Quais dados a extensão acessa
Usando a sua própria sessão autenticada, a extensão consulta, via API do Dynamics 365, apenas o necessário para o seu trabalho:
* Ocorrências (casos) abertas atribuídas a você: número, assunto, prazo de SLA, número do pedido e valor (quando configurados);
* Dados de contato/cliente vinculados à ocorrência (nome e e-mail), para preencher o destinatário;
* E-mails recebidos vinculados à ocorrência (assunto e um resumo), para avisar sobre novas mensagens do cliente;
* A fila de envio, para enviar o e-mail em seu nome a partir dela.

Esses dados já são acessíveis a você dentro do Dynamics; a extensão apenas os exibe de forma mais prática. Eles são buscados ao vivo e mostrados na tela — não são transmitidos para fora.

## 3. O que é armazenado localmente
Para funcionar, a extensão guarda **apenas no seu próprio dispositivo** (`chrome.storage.local`) os seguintes itens, que nunca são enviados a lugar nenhum:
* Suas configurações (fila, campos mapeados, modelos de e-mail, logo e assinatura);
* As ocorrências que você fixou como prioridade (apenas o identificador do caso);
* Suas observações pessoais sobre cada caso (texto escrito por você);
* Marcações de "e-mail já visto" (apenas data/hora), para controlar o aviso de novidade.

**Nenhum endereço de e-mail ou conteúdo de mensagem do cliente é gravado.** Esses dados são exibidos de forma transitória e descartados ao fechar a extensão.

## 4. Permissões e por que são usadas
* `activeTab` / `scripting`: ler a ocorrência aberta e enviar o e-mail pela API, na própria página do Dynamics;
* `storage`: salvar suas configurações e preferências localmente;
* `alarms` e `notifications`: verificar periodicamente novos e-mails do cliente e te avisar;
* `optional_host_permissions` (domínios do Dynamics): concedida por você, permite o aviso de novos e-mails em segundo plano.

## 5. Compartilhamento de dados
A extensão **não compartilha, vende ou transfere** dados a terceiros. Não há comunicação com servidores do desenvolvedor. Todo o tratamento ocorre localmente e contra a API do Dynamics 365 da sua organização.

## 6. LGPD
Por processar dados pessoais apenas localmente, dentro do acesso que você já possui de forma legítima ao Dynamics, e sem transmissão a terceiros, a extensão foi desenhada para respeitar a Lei Geral de Proteção de Dados (LGPD). Há ainda uma opção para ocultar parcialmente o e-mail do cliente na tela, como camada extra de privacidade.

## 7. Retenção e exclusão
Os dados armazenados localmente permanecem no seu dispositivo até você removê-los. Você pode apagar tudo a qualquer momento em *Configurações → Restaurar padrão*, ou removendo a extensão do navegador.

## 8. Contato
Em caso de dúvidas sobre esta Política de Privacidade, entre em contato:

**Desenvolvedor:** Alisson Rozendo Dos Santos  
**E-mail:** alisson.rozendo1998@gmail.com  
**Repositório:** [https://github.com/Alisson790br/Fapp-monitor-e-mail](https://github.com/Alisson790br/Fapp-monitor-e-mail)
