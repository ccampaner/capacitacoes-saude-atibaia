# Portal de Capacitações Interativas • Secretarias Municipais de Saúde

Repositório estático desenvolvido para hospedagem gratuita no **GitHub Pages**, contendo o menu inicial (`index.html`), 3 capacitações interativas (5 módulos cada, avaliação por módulo, salvamento automático no navegador via `localStorage`, **Pesquisa de Satisfação integrada** e emissão de **Certificado em PDF A4 Paisagem** com 3 horas de carga horária) e o script de coleta de feedback (`google_apps_script_feedback.gs`).

## Capacitações Disponíveis

1. **`capacitacao_IA_saude.html`** — Inteligência Artificial Aplicada à Gestão e Rotina do SUS (5 Módulos • 03h)
2. **`capacitacao_lei_8080_sus.html`** — Lei Orgânica da Saúde: Lei Federal nº 8.080/1990 (5 Módulos • 03h)
3. **`capacitacao_LGPD_saude.html`** — Lei Geral de Proteção de Dados (LGPD) Aplicada à Rotina da Saúde (5 Módulos • 03h)

## Como ativar a gravação da Pesquisa de Satisfação no Google Sheets

1. Acesse [sheets.new](https://sheets.new) e crie uma nova Planilha Google (ex.: `Feedback Capacitacoes Saude`).
2. No menu superior da planilha, clique em **Extensões → Apps Script**.
3. Apague o código padrão e cole o conteúdo do arquivo **`google_apps_script_feedback.gs`**.
4. Clique em **Implantar → Nova implantação → Tipo: App da Web**:
   - **Executar como:** `Eu`
   - **Quem pode acessar:** `Qualquer pessoa`
5. Copie a **URL do App da Web** gerada (terminada em `/exec`).
6. Nos 3 arquivos HTML dos cursos, localize a linha `const FEEDBACK_WEBHOOK_URL = "";` e cole a URL entre as aspas.

## Contato

Desenvolvido para Secretarias Municipais de Saúde — `clovis_campaner@yahoo.com.br`
