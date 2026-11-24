# eBook Maker

> Gere eBooks profissionais com capas geradas por IA em minutos. Zero conhecimento tÃ©cnico necessÃ¡rio.

![Capa de Exemplo](sample/cover_image.png)

---

## Para Iniciantes: Use com Claude Code (Mais FÃ¡cil!)

Se vocÃª tem o **Claude Code** instalado, nÃ£o precisa fazer nada manual. Basta dizer:

> "Crie um ebook sobre [seu tÃ³pico]"

O Claude faz todo o trabalho automaticamente!

**NÃ£o tem Claude Code?** [Instale aqui](https://claude.ai/code) e siga o tutorial abaixo.

---

## Tutorial Completo para Leigos (Passo a Passo)

### O Que VocÃª Vai Precisar

| Ferramenta | Para Que Serve | Link |
|------------|----------------|------|
| **Claude Code** | Assistente IA que cria o eBook | [claude.ai/code](https://claude.ai/code) |
| **Conta Google** | Para gerar imagens de capa | VocÃª jÃ¡ tem! |

### Passo 1: Instalar o Claude Code

1. Acesse [claude.ai/code](https://claude.ai/code)
2. Baixe o instalador para seu sistema (Windows/Mac/Linux)
3. Execute o instalador e siga as instruÃ§Ãµes
4. Abra o terminal e digite `claude` para verificar se funcionou

### Passo 2: Baixar Este Projeto

Abra o terminal e digite:

```bash
git clone https://github.com/linnoff88-dev/ebook-maker.git
cd ebook-maker
```

### Passo 3: Obter Chave da API do Google (GrÃ¡tis)

1. Acesse [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
2. FaÃ§a login com sua conta Google
3. Clique em **"Create API Key"**
4. Copie a chave gerada (parece com: `AIzaSy...`)

### Passo 4: Iniciar o Claude Code

No terminal, dentro da pasta do projeto:

```bash
claude
```

### Passo 5: Configurar e Criar Seu eBook

Agora Ã© sÃ³ conversar com o Claude! Diga:

> "Configure a chave da API: [cole sua chave aqui]"

Depois:

> "Crie um ebook sobre [seu tema]"

**Exemplo:**
> "Crie um ebook sobre Marketing Digital para Pequenas Empresas"

O Claude vai:
1. Perguntar o tÃ­tulo e subtÃ­tulo
2. Gerar uma capa profissional com IA
3. Criar todo o conteÃºdo formatado
4. Exportar para PDF

**Pronto! Seu eBook estarÃ¡ na pasta `output/`**

---

## 3 Layouts DisponÃ­veis

Este projeto inclui 3 estilos de layout profissionais:

### 1. Editorial ClÃ¡ssico
**Arquivo:** `layout_editorial_classico.js`

**Ideal para:** Romances, biografias, livros de histÃ³ria

**CaracterÃ­sticas:**
- Fonte serifada elegante (Georgia)
- Capitulares decorativas (letra grande no inÃ­cio)
- EpÃ­grafes (citaÃ§Ãµes no inÃ­cio dos capÃ­tulos)
- Margens largas com proporÃ§Ã£o clÃ¡ssica
- Ornamentos tipogrÃ¡ficos (â¦)
- NumeraÃ§Ã£o de pÃ¡gina centralizada

**InspiraÃ§Ã£o:** Penguin Classics, livros da Companhia das Letras

```
+------------------------+
|                        |
|    CAPÃTULO I          |
|    O InÃ­cio            |
|         â§              |
|  "CitaÃ§Ã£o elegante"    |
|      â€” Autor           |
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

**CaracterÃ­sticas:**
- Fonte sans-serif limpa (Arial)
- Caixas coloridas de destaque (Dicas, Avisos, Resumos)
- Listas e bullets bem definidos
- CabeÃ§alhos numerados com linhas divisÃ³rias
- Foco em escaneabilidade e aprendizado rÃ¡pido

**InspiraÃ§Ã£o:** Livros da O'Reilly, A Book Apart

```
+------------------------+
|  GUIA PRÃTICO      P.4 |
|  ________________      |
|                        |
|  # 1. O Conceito       |
|                        |
|  +------------------+  |
|  | ðŸ’¡ DICA:         |  |
|  | Sempre comece... |  |
|  +------------------+  |
|                        |
|  â€¢ Item 1              |
|  â€¢ Item 2              |
|  â€¢ Item 3              |
|                        |
+------------------------+
```

---

### 3. Minimalista SuÃ­Ã§o
**Arquivo:** `layout_minimalista_suico.js`

**Ideal para:** PortfÃ³lios, manifestos, livros de design/arquitetura

**CaracterÃ­sticas:**
- Grid assimÃ©trico (coluna de notas + texto principal)
- Muito espaÃ§o em branco intencional
- TÃ­tulos gigantes em negrito
- Apenas preto, branco e cinza
- Texto alinhado Ã  esquerda (nunca justificado)

**InspiraÃ§Ã£o:** Josef MÃ¼ller-Brockmann, Vignelli Canon

```
+------------------------+
|                        |
|  01.                   |
|  A BASE                |
|                        |
|  Nota:     O design    |
|            nÃ£o Ã© sÃ³    |
|            aparÃªncia.  |
|                        |
|            Ã‰ funÃ§Ã£o.   |
|                        |
|                        |
|  2                     |
+------------------------+
```

---

## Como Usar os Layouts

### MÃ©todo 1: Via Claude Code (Recomendado)

Simplesmente peÃ§a ao Claude:

> "Crie um eBook usando o layout Editorial ClÃ¡ssico sobre [tema]"

ou

> "Use o layout Moderno Funcional para criar um guia sobre [tema]"

ou

> "Quero um eBook estilo Minimalista SuÃ­Ã§o sobre [tema]"

### MÃ©todo 2: Executar Diretamente

```bash
# Entrar na pasta do projeto
cd ebook-maker/ai_report_package

# Gerar com Layout Editorial ClÃ¡ssico
node layout_editorial_classico.js

# Gerar com Layout Moderno Funcional
node layout_moderno_funcional.js

# Gerar com Layout Minimalista SuÃ­Ã§o
node layout_minimalista_suico.js

# Converter para PDF (Linux)
libreoffice --headless --convert-to pdf ../output/Layout_Editorial_Classico.docx
```

### MÃ©todo 3: Personalizar o Layout

Cada arquivo de layout exporta funÃ§Ãµes reutilizÃ¡veis. Exemplo com Editorial ClÃ¡ssico:

```javascript
const {
  createChapterTitle,  // TÃ­tulo de capÃ­tulo elegante
  createEpigraph,      // CitaÃ§Ã£o no inÃ­cio
  createDropCap,       // Capitular decorativa
  createParagraph,     // ParÃ¡grafo com indentaÃ§Ã£o
  createSectionBreak   // Separador * * *
} = require('./layout_editorial_classico.js');

// Use as funÃ§Ãµes para criar seu conteÃºdo personalizado
```

---

## Estrutura do Projeto

```
ebook-maker/
â”œâ”€â”€ ai_report_package/
â”‚   â”œâ”€â”€ create_report.js              # Layout McKinsey (padrÃ£o)
â”‚   â”œâ”€â”€ layout_editorial_classico.js  # Layout 1: Romances
â”‚   â”œâ”€â”€ layout_moderno_funcional.js   # Layout 2: Guias/Tutoriais
â”‚   â”œâ”€â”€ layout_minimalista_suico.js   # Layout 3: Design/PortfÃ³lio
â”‚   â”œâ”€â”€ logo.png
â”‚   â””â”€â”€ package.json
â”œâ”€â”€ .claude/
â”‚   â””â”€â”€ skills/
â”‚       â””â”€â”€ ebook-creator.md          # Skill do Claude Code
â”œâ”€â”€ output/                           # Arquivos gerados
â”œâ”€â”€ sample/                           # Exemplos
â”œâ”€â”€ generate_image.py                 # Gerador de capas com IA
â”œâ”€â”€ requirements.txt
â”œâ”€â”€ CLAUDE.md
â””â”€â”€ README.md
```

---

## InstalaÃ§Ã£o Manual (Para Desenvolvedores)

Se preferir nÃ£o usar o Claude Code:

### PrÃ©-requisitos

- Node.js v16+ â€” [nodejs.org](https://nodejs.org/)
- Python 3.8+ â€” [python.org](https://python.org/)
- LibreOffice â€” [libreoffice.org](https://libreoffice.org/)

### InstalaÃ§Ã£o

```bash
# Clonar repositÃ³rio
git clone https://github.com/linnoff88-dev/ebook-maker.git
cd ebook-maker

# Configurar API
echo "GEMINI_API_KEY=sua_chave_aqui" > .env

# Instalar dependÃªncias Python
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

# Instalar dependÃªncias Node.js
cd ai_report_package && npm install && cd ..

# Criar pasta de saÃ­da
mkdir -p output
```

### Gerar eBook

```bash
# 1. Gerar imagem de capa
source venv/bin/activate && python generate_image.py

# 2. Gerar documento (escolha um layout)
cd ai_report_package
node create_report.js                  # McKinsey (padrÃ£o)
# ou
node layout_editorial_classico.js      # ClÃ¡ssico
# ou
node layout_moderno_funcional.js       # Funcional
# ou
node layout_minimalista_suico.js       # Minimalista

# 3. Converter para PDF
cd ..
libreoffice --headless --convert-to pdf output/*.docx
```

---

## PersonalizaÃ§Ã£o AvanÃ§ada

### Alterar Cores

Cada layout tem constantes de cor no topo do arquivo:

**Editorial ClÃ¡ssico:**
```javascript
const DARK_BROWN = "3D2914";
const GOLD = "8B7355";
```

**Moderno Funcional:**
```javascript
const PRIMARY_BLUE = "0066CC";
const ACCENT_ORANGE = "FF6600";
```

**Minimalista SuÃ­Ã§o:**
```javascript
const BLACK = "000000";
const MEDIUM_GRAY = "999999";
```

### Alterar Fontes

Procure por `font: "Georgia"` ou `font: "Arial"` e substitua por:
- Serifadas: `"Times New Roman"`, `"Garamond"`, `"Palatino"`
- Sans-serif: `"Helvetica"`, `"Roboto"`, `"Open Sans"`

### Adicionar Novas SeÃ§Ãµes

Use as funÃ§Ãµes auxiliares de cada layout:

```javascript
// Editorial ClÃ¡ssico
createChapterTitle("III", "Novo CapÃ­tulo")
createEpigraph("CitaÃ§Ã£o inspiradora", "Autor")
createDropCap("A", "qui comeÃ§a o texto...")

// Moderno Funcional
createSectionHeader("03", "NOVA SEÃ‡ÃƒO")
createTipBox("DICA", "ConteÃºdo da dica")
createWarningBox("Aviso importante!")
createSummaryBox(["Item 1", "Item 2", "Item 3"])

// Minimalista SuÃ­Ã§o
createSectionTitle("03.", "NOVO TEMA")
createTwoColumnLayout("Nota lateral", "Texto principal aqui")
createQuote("CitaÃ§Ã£o impactante")
```

---

## SoluÃ§Ã£o de Problemas

### "Module not found"
```bash
cd ai_report_package && npm install
```

### "GEMINI_API_KEY not found"
```bash
echo "GEMINI_API_KEY=sua_chave" > .env
```

### PDF nÃ£o gera
```bash
# Linux
sudo apt install libreoffice

# macOS
brew install libreoffice
```

### Imagem de capa nÃ£o aparece
Certifique-se de que existe `output/cover_image.png` antes de rodar o layout.

---

## Exemplos de Prompts para o Claude

```
"Crie um eBook sobre InteligÃªncia Artificial para Iniciantes"

"Use o layout Editorial ClÃ¡ssico para criar um livro de poesias"

"Gere um guia prÃ¡tico de Marketing Digital com layout Moderno Funcional"

"Crie um portfÃ³lio minimalista sobre Design de Interiores"

"FaÃ§a um eBook sobre Produtividade com capa azul e dourada"
```

---

## Stack TecnolÃ³gica

| Componente | Tecnologia |
|------------|------------|
| GeraÃ§Ã£o de Capa | Google Gemini 3 Pro Image |
| CriaÃ§Ã£o de Documento | Node.js + [docx](https://www.npmjs.com/package/docx) |
| ExportaÃ§Ã£o PDF | LibreOffice (headless) |
| Assistente IA | Claude Code |

---

## LicenÃ§a

MIT â€” use como quiser.

---

<p align="center">
  <b>ConstruÃ­do com Claude Code</b><br>
  <a href="https://claude.ai/code">claude.ai/code</a>
</p>

---

Projeto adaptado da comunidade ARCKHÉ TDS - Marca Arckhe