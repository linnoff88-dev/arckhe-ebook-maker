# eBook Maker

> Gere eBooks profissionais com capas geradas por IA em minutos. Zero conhecimento têÂ©cnico necessêÂ¡rio.

![Capa de Exemplo](sample/cover_image.png)

---

## Para Iniciantes: Use com Claude Code (Mais FêÂ¡cil!)

Se vocêÂª tem o **Claude Code** instalado, nêÂ£o precisa fazer nada manual. Basta dizer:

> "Crie um ebook sobre [seu têÂ³pico]"

O Claude faz todo o trabalho automaticamente!

**NêÂ£o tem Claude Code?** [Instale aqui](https://claude.ai/code) e siga o tutorial abaixo.

---

## Tutorial Completo para Leigos (Passo a Passo)

### O Que VocêÂª Vai Precisar

| Ferramenta | Para Que Serve | Link |
|------------|----------------|------|
| **Claude Code** | Assistente IA que cria o eBook | [claude.ai/code](https://claude.ai/code) |
| **Conta Google** | Para gerar imagens de capa | VocêÂª jêÂ¡ tem! |

### Passo 1: Instalar o Claude Code

1. Acesse [claude.ai/code](https://claude.ai/code)
2. Baixe o instalador para seu sistema (Windows/Mac/Linux)
3. Execute o instalador e siga as instruêÂ§êÂµes
4. Abra o terminal e digite `claude` para verificar se funcionou

### Passo 2: Baixar Este Projeto

Abra o terminal e digite:

```bash
git clone https://github.com/linnoff88-dev/ebook-maker.git
cd ebook-maker
```

### Passo 3: Obter Chave da API do Google (GrêÂ¡tis)

1. Acesse [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. FaêÂ§a login com sua conta Google
3. Clique em **"Create API Key"**
4. Copie a chave gerada (parece com: `AIzaSy...`)

### Passo 4: Iniciar o Claude Code

No terminal, dentro da pasta do projeto:

```bash
claude
```

### Passo 5: Configurar e Criar Seu eBook

Agora êÂ© sêÂ³ conversar com o Claude! Diga:

> "Configure a chave da API: [cole sua chave aqui]"

Depois:

> "Crie um ebook sobre [seu tema]"

**Exemplo:**
> "Crie um ebook sobre Marketing Digital para Pequenas Empresas"

O Claude vai:
1. Perguntar o têÂ­tulo e subtêÂ­tulo
2. Gerar uma capa profissional com IA
3. Criar todo o conteêÂºdo formatado
4. Exportar para PDF

**Pronto! Seu eBook estarêÂ¡ na pasta `output/`**

---

## 3 Layouts DisponêÂ­veis

Este projeto inclui 3 estilos de layout profissionais:

### 1. Editorial ClêÂ¡ssico
**Arquivo:** `layout_editorial_classico.js`

**Ideal para:** Romances, biografias, livros de histêÂ³ria

**CaracterêÂ­sticas:**
- Fonte serifada elegante (Georgia)
- Capitulares decorativas (letra grande no inêÂ­cio)
- EpêÂ­grafes (citaêÂ§êÂµes no inêÂ­cio dos capêÂ­tulos)
- Margens largas com proporêÂ§êÂ£o clêÂ¡ssica
- Ornamentos tipogrêÂ¡ficos (ê¢ÂÂ¦)
- NumeraêÂ§êÂ£o de pêÂ¡gina centralizada

**InspiraêÂ§êÂ£o:** Penguin Classics, livros da Companhia das Letras

```
+------------------------+
|                        |
|    CAPêÂTULO I          |
|    O InêÂ­cio            |
|         ê¢ÂÂ§              |
|  "CitaêÂ§êÂ£o elegante"    |
|      ê¢â¬â Autor           |
|                        |
|  ERA uma vez, em um    |
|  reino distante...     |
|                        |
|         12             |
+------------------------+
```

---

### 2. Moderno Funcional
**Arquivo:** `layout_moderno_funcional.js`

**Ideal para:** Guias, tutoriais, eBooks de marketing, manuais

**CaracterêÂ­sticas:**
- Fonte sans-serif limpa (Arial)
- Caixas coloridas de destaque (Dicas, Avisos, Resumos)
- Listas e bullets bem definidos
- CabeêÂ§alhos numerados com linhas divisêÂ³rias
- Foco em escaneabilidade e aprendizado rêÂ¡pido

**InspiraêÂ§êÂ£o:** Livros da O'Reilly, A Book Apart

```
+------------------------+
|  GUIA PRêÂTICO      P.4 |
|  ________________      |
|                        |
|  # 1. O Conceito       |
|                        |
|  +------------------+  |
|  | ê°Å¸âÂ¡ DICA:         |  |
|  | Sempre comece... |  |
|  +------------------+  |
|                        |
|  ê¢â¬Â¢ Item 1              |
|  ê¢â¬Â¢ Item 2              |
|  ê¢â¬Â¢ Item 3              |
|                        |
+------------------------+
```

---

### 3. Minimalista SuêÂ­êÂ§o
**Arquivo:** `layout_minimalista_suico.js`

**Ideal para:** PortfêÂ³lios, manifestos, livros de design/arquitetura

**CaracterêÂ­sticas:**
- Grid assimêÂ©trico (coluna de notas + texto principal)
- Muito espaêÂ§o em branco intencional
- TêÂ­tulos gigantes em negrito
- Apenas preto, branco e cinza
- Texto alinhado êÂ  esquerda (nunca justificado)

**InspiraêÂ§êÂ£o:** Josef MêÂ¼ller-Brockmann, Vignelli Canon

```
+------------------------+
|                        |
|  01.                   |
|  A BASE                |
|                        |
|  Nota:     O design    |
|            nêÂ£o êÂ© sêÂ³    |
|            aparêÂªncia.  |
|                        |
|            êâ° funêÂ§êÂ£o.   |
|                        |
|                        |
|  2                     |
+------------------------+
```

---

## Como Usar os Layouts

### MêÂ©todo 1: Via Claude Code (Recomendado)

Simplesmente peêÂ§a ao Claude:

> "Crie um eBook usando o layout Editorial ClêÂ¡ssico sobre [tema]"

ou

> "Use o layout Moderno Funcional para criar um guia sobre [tema]"

ou

> "Quero um eBook estilo Minimalista SuêÂ­êÂ§o sobre [tema]"

### MêÂ©todo 2: Executar Diretamente

```bash
# Entrar na pasta do projeto
cd ebook-maker/ai_report_package

# Gerar com Layout Editorial ClêÂ¡ssico
node layout_editorial_classico.js

# Gerar com Layout Moderno Funcional
node layout_moderno_funcional.js

# Gerar com Layout Minimalista SuêÂ­êÂ§o
node layout_minimalista_suico.js

# Converter para PDF (Linux)
libreoffice --headless --convert-to pdf ../output/Layout_Editorial_Classico.docx
```

### MêÂ©todo 3: Personalizar o Layout

Cada arquivo de layout exporta funêÂ§êÂµes reutilizêÂ¡veis. Exemplo com Editorial ClêÂ¡ssico:

```javascript
const {
  createChapterTitle,  // TêÂ­tulo de capêÂ­tulo elegante
  createEpigraph,      // CitaêÂ§êÂ£o no inêÂ­cio
  createDropCap,       // Capitular decorativa
  createParagraph,     // ParêÂ¡grafo com indentaêÂ§êÂ£o
  createSectionBreak   // Separador * * *
} = require('./layout_editorial_classico.js');

// Use as funêÂ§êÂµes para criar seu conteêÂºdo personalizado
```

---

## Estrutura do Projeto

```
ebook-maker/
ê¢âÅê¢ââ¬ê¢ââ¬ ai_report_package/
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ create_report.js              # Layout McKinsey (padrêÂ£o)
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ layout_editorial_classico.js  # Layout 1: Romances
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ layout_moderno_funcional.js   # Layout 2: Guias/Tutoriais
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ layout_minimalista_suico.js   # Layout 3: Design/PortfêÂ³lio
ê¢ââ   ê¢âÅê¢ââ¬ê¢ââ¬ logo.png
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ package.json
ê¢âÅê¢ââ¬ê¢ââ¬ .claude/
ê¢ââ   ê¢ââê¢ââ¬ê¢ââ¬ skills/
ê¢ââ       ê¢ââê¢ââ¬ê¢ââ¬ ebook-creator.md          # Skill do Claude Code
ê¢âÅê¢ââ¬ê¢ââ¬ output/                           # Arquivos gerados
ê¢âÅê¢ââ¬ê¢ââ¬ sample/                           # Exemplos
ê¢âÅê¢ââ¬ê¢ââ¬ generate_image.py                 # Gerador de capas com IA
ê¢âÅê¢ââ¬ê¢ââ¬ requirements.txt
ê¢âÅê¢ââ¬ê¢ââ¬ CLAUDE.md
ê¢ââê¢ââ¬ê¢ââ¬ README.md
```

---

## InstalaêÂ§êÂ£o Manual (Para Desenvolvedores)

Se preferir nêÂ£o usar o Claude Code:

### PrêÂ©-requisitos

- Node.js v16+ ê¢â¬â [nodejs.org](https://nodejs.org/)
- Python 3.8+ ê¢â¬â [python.org](https://python.org/)
- LibreOffice ê¢â¬â [libreoffice.org](https://libreoffice.org/)

### InstalaêÂ§êÂ£o

```bash
# Clonar repositêÂ³rio
git clone https://github.com/linnoff88-dev/ebook-maker.git
cd ebook-maker

# Configurar API
echo "GEMINI_API_KEY=sua_chave_aqui" > .env

# Instalar dependêÂªncias Python
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Instalar dependêÂªncias Node.js
cd ai_report_package && npm install && cd ..

# Criar pasta de saêÂ­da
mkdir -p output
```

### Gerar eBook

```bash
# 1. Gerar imagem de capa
source venv/bin/activate && python generate_image.py

# 2. Gerar documento (escolha um layout)
cd ai_report_package
node create_report.js                  # McKinsey (padrêÂ£o)
# ou
node layout_editorial_classico.js      # ClêÂ¡ssico
# ou
node layout_moderno_funcional.js       # Funcional
# ou
node layout_minimalista_suico.js       # Minimalista

# 3. Converter para PDF
cd ..
libreoffice --headless --convert-to pdf output/*.docx
```

---

## PersonalizaêÂ§êÂ£o AvanêÂ§ada

### Alterar Cores

Cada layout tem constantes de cor no topo do arquivo:

**Editorial ClêÂ¡ssico:**
```javascript
const DARK_BROWN = "3D2914";
const GOLD = "8B7355";
```

**Moderno Funcional:**
```javascript
const PRIMARY_BLUE = "0066CC";
const ACCENT_ORANGE = "FF6600";
```

**Minimalista SuêÂ­êÂ§o:**
```javascript
const BLACK = "000000";
const MEDIUM_GRAY = "999999";
```

### Alterar Fontes

Procure por `font: "Georgia"` ou `font: "Arial"` e substitua por:
- Serifadas: `"Times New Roman"`, `"Garamond"`, `"Palatino"`
- Sans-serif: `"Helvetica"`, `"Roboto"`, `"Open Sans"`

### Adicionar Novas SeêÂ§êÂµes

Use as funêÂ§êÂµes auxiliares de cada layout:

```javascript
// Editorial ClêÂ¡ssico
createChapterTitle("III", "Novo CapêÂ­tulo")
createEpigraph("CitaêÂ§êÂ£o inspiradora", "Autor")
createDropCap("A", "qui comeêÂ§a o texto...")

// Moderno Funcional
createSectionHeader("03", "NOVA SEêâ¡êÆO")
createTipBox("DICA", "ConteêÂºdo da dica")
createWarningBox("Aviso importante!")
createSummaryBox(["Item 1", "Item 2", "Item 3"])

// Minimalista SuêÂ­êÂ§o
createSectionTitle("03.", "NOVO TEMA")
createTwoColumnLayout("Nota lateral", "Texto principal aqui")
createQuote("CitaêÂ§êÂ£o impactante")
```

---

## SoluêÂ§êÂ£o de Problemas

### "Module not found"
```bash
cd ai_report_package && npm install
```

### "GEMINI_API_KEY not found"
```bash
echo "GEMINI_API_KEY=sua_chave" > .env
```

### PDF nêÂ£o gera
```bash
# Linux
sudo apt install libreoffice

# macOS
brew install libreoffice
```

### Imagem de capa nêÂ£o aparece
Certifique-se de que existe `output/cover_image.png` antes de rodar o layout.

---

## Exemplos de Prompts para o Claude

```
"Crie um eBook sobre InteligêÂªncia Artificial para Iniciantes"

"Use o layout Editorial ClêÂ¡ssico para criar um livro de poesias"

"Gere um guia prêÂ¡tico de Marketing Digital com layout Moderno Funcional"

"Crie um portfêÂ³lio minimalista sobre Design de Interiores"

"FaêÂ§a um eBook sobre Produtividade com capa azul e dourada"
```

---

## Stack TecnolêÂ³gica

| Componente | Tecnologia |
|------------|------------|
| GeraêÂ§êÂ£o de Capa | Google Gemini 3 Pro Image |
| CriaêÂ§êÂ£o de Documento | Node.js + [docx](https://www.npmjs.com/package/docx) |
| ExportaêÂ§êÂ£o PDF | LibreOffice (headless) |
| Assistente IA | Claude Code |

---

## LicenêÂ§a

MIT ê¢â¬â use como quiser.

---

<p align="center">
  <b>ConstruêÂ­do com Claude Code</b><br>
  <a href="https://claude.ai/code">claude.ai/code</a>
</p>

---

Projeto adaptado da comunidade ARCKHê TDS - ARCKHÉe