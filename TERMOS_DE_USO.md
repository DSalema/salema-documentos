# Termos de Uso e Condições Gerais
**Aplicativo Salema — Diário de Serviços**
*Versão do Documento: 1.0.0 — Setembro de 2026*

Seja bem-vindo ao **Salema — Diário de Serviços**. Este documento estabelece as regras, condições e obrigações para a utilização do nosso software. Ao instalar e utilizar o aplicativo, você concorda integralmente com estes Termos de Uso.

---

### 1. Objeto e Escopo Operacional
O Salema é um aplicativo móvel voltado para o registro técnico de atividades em campo, com captura de evidências fotográficas, indexação automatizada de coordenadas geográficas via GPS e exportação de relatórios estruturados em formatos PDF e Excel (.xlsx).

### 2. Modalidades de Licenciamento (Planos)
O aplicativo opera sob um modelo híbrido local, contendo duas modalidades:
* **Plano Gratuito (Free):** Concede o direito de registrar dados de forma local. Os relatórios em formato PDF são limitados estritamente a no máximo 3 (três) registros por arquivo de amostragem e incluem obrigatoriamente uma marca d'água institucional. A exportação para planilhas em formato Excel (.xlsx) e a customização de cabeçalhos e logomarcas permanecem bloqueadas.
* **Plano Premium:** Desbloqueia relatórios em PDF sem limites de registros, exportação estruturada para planilhas Excel (.xlsx) com injeção binária de imagens e ferramentas avançadas de customização visual (logotipo da empresa, título de cabeçalho e rodapé).

### 3. Mecanismo de Validação Criptográfica Offline e Segurança
* A ativação do Plano Premium ocorre por meio de uma chave de liberação comercial gerada pelo aplicativo administrador exclusivo.
* Esta chave é vinculada de forma indissociável ao par de dados composto pelo **E-mail de Cadastro Funcional** e pelo **ID de Hardware (ID físico)** do dispositivo móvel do usuário.
* O algoritmo de validação opera de forma 100% offline e descentralizada, realizando o cálculo criptográfico síncrono e desembaralhando os bits com base no dia civil do fuso horário bruto unificado.
* Tentativas de engenharia reversa, manipulação do relógio do sistema para burlar prazos ou compartilhamento indevido de chaves resultarão na revogação permanente do acesso Premium sem aviso prévio.

### 4. Controle de Abuso e Trava Antispam
Para garantir a estabilidade do suporte técnico e evitar sobrecarga na infraestrutura de atendimento via WhatsApp, o aplicativo possui uma trava rígida temporizada. Após o envio de uma solicitação de chave técnica ao representante, o botão de redirecionamento permanecerá bloqueado por exatamente **01 (uma) hora**, exibindo uma contagem regressiva em tela. Adicionalmente, caso o aparelho já possua uma licença Premium válida e ativa, o botão do WhatsApp será permanentemente trancado até o vencimento da mesma.

### 5. Regras de Remoção Severa e Período de Carência
O usuário possui total autonomia para remover a licença ativa por meio do botão de exclusão técnica severa no rodapé do app, exigindo duplo fator de confirmação. 
* **Prazo de Carência de 24 Horas:** No momento em que uma chave Premium expira ou é removida manualmente pelo usuário para fins de upgrade de plano, as customizações salvas (logotipo, cabeçalho e rodapé) entram em uma contagem regressiva temporal de carência de segurança.
* As customizações continuarão funcionando normalmente por exatamente **24 horas**. Passado este prazo exato, o sistema executará uma limpeza automática nos registros do SharedPreferences locais, redefinindo o design do documento PDF para o padrão gratuito (Free).

### 6. Limitação de Responsabilidade
O Salema opera de forma local e offline (`sqflite` e `SharedPreferences`). O aplicativo não realiza backup em nuvem automática dos diários de serviços. A guarda, exclusão manual diária ("Zerar Histórico") e integridade dos dados gerados, relatórios e fotos salvos no armazenamento interno do Android são de inteira e exclusiva responsabilidade do usuário.

### 7. Alterações nos Termos
Reservamo-nos o direito de atualizar este documento a qualquer momento para refletir melhorias no motor criptográfico ou na arquitetura de software. O uso contínuo do app constitui aceitação dos novos termos.

---
Dalton Ferreira Salema  
Desenvolvedor Responsável  
Contato: daltonsalema26@gmail.com
