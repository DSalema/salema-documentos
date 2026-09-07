# Política de Privacidade e Proteção de Dados
**Aplicativo Salema — Diário de Serviços**
*Versão do Documento: 1.0.0 — Setembro de 2026*

Sua privacidade e a segurança dos dados de campo coletados são pilares fundamentais do desenvolvimento do aplicativo **Salema — Diário de Serviços**. Esta Política de Privacidade explica como o software lida com as suas informações técnicas.

---

### 1. Arquitetura 100% Offline e Armazenamento Local
O Salema foi projetado sob a premissa de soberania de dados do usuário. O aplicativo **não possui servidores de nuvem próprios e não faz upload** de suas fotos, textos, detalhamentos técnicos ou localização para redes de terceiros.
* Os registros textuais do seu diário de serviços são armazenados localmente em um banco de dados relacional criptografado internamente via pacote `sqflite`.
* As imagens capturadas são salvas no diretório físico interno de dados do Android gerenciado pelo sistema operacional.
* Configurações de planos e personalizações visuais são gravadas localmente através do mecanismo `SharedPreferences`.

### 2. Permissões de Hardware Coletadas e Finalidade
Para exercer suas funções técnicas de engenharia e auditoria, o aplicativo requer acesso restrito a componentes de hardware:
* **Geolocalização por GPS de Alta Precisão (`Geolocator`):** Coleta as coordenadas de latitude e longitude em tempo real (calibradas com até 8 casas decimais). Essas coordenadas são capturadas única e exclusivamente no exato instante em que o fiscal dispara a câmera ou seleciona uma imagem da galeria, sendo injetadas de forma permanente nos metadados do relatório Excel e na folha física do PDF para fins de comprovação técnica de execução. O rastreamento cessa ao fechar a aplicação.
* **Câmera e Armazenamento/Galeria (`ImagePicker`):** Necessários para a captura e anexação das 3 (três) evidências fotográficas obrigatórias por registro de serviço, além do carregamento do logotipo corporativo personalizado no Plano Premium.

### 3. Higienização e Tratamento da Identidade do Dispositivo
Para fins de validação da licença de uso do Plano Premium, o aplicativo realiza a leitura do ID físico do dispositivo Android (`device_info_plus`).
* **Filtro Alfanumérico Puro Estrito:** Visando eliminar inconsistências e quebras de segurança causadas por formatações específicas de fabricantes (como pontos estruturais em linhas Samsung M31), o aplicativo e o painel administrador aplicam uma expressão regular rigorosa (`[^a-z0-9]`). 
* Esse filtro higieniza e converte tanto o E-mail de Cadastro Funcional quanto o ID do Hardware em cadeias alfanuméricas limpas e síncronas antes da execução do laço criptográfico de desembaralhamento de dados.

### 4. Retenção e Exclusão de Dados
* **Zerar Histórico Manual:** O usuário possui controle absoluto sobre o tempo de retenção das informações. Através do botão "Zerar Histórico" (ícone da lixeira) no menu inferior, o aplicativo realiza a exclusão em cascata completa de todas as fotos e registros de diário salvos no SQLite, limpando o banco local de forma imediata e irrecuperável.
* **Detecção Automática de Novo Dia Civil:** Ao abrir o aplicativo, o sistema checa o timestamp do último acesso. Caso detecte a mudança para um novo dia civil, o app exibe uma janela de alerta oferecendo a limpeza do lote de dados de dias anteriores para manter o painel técnico higienizado.

### 5. Compartilhamento de Arquivos por Ações do Usuário
O compartilhamento dos relatórios PDF e planilhas Excel compiladas ocorre unicamente por ação deliberada do usuário, por meio do acionamento dos botões de exportação integrados ao pacote `share_plus`. Os arquivos são empacotados localmente no diretório temporário do Android e transferidos para o aplicativo de destino escolhido pelo usuário (como o WhatsApp).

### 6. Contato e Suporte Técnico
Para esclarecimentos sobre a arquitetura de dados do software ou suporte para ativação do Plano Premium, entre em contato diretamente com o desenvolvedor responsável:

Dalton Ferreira Salema  
E-mail Técnico: daltonsalema26@gmail.com
