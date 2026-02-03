# G6PD Research Initiative Website

A professional research website showcasing G6PD deficiency research, AlphaFold protein analysis, and CRISPR-Cas9 therapeutic potential.

**Author:** Luke Chen
**Domain:** G6PDResearch.org

---

## Quick Start - Deploy to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Name it: `g6pdresearch.org` (or any name you prefer)
4. Make it **Public**
5. Click **Create repository**

### Step 2: Upload Files

1. In your new repository, click **uploading an existing file**
2. Drag and drop `index.html` into the upload area
3. Add commit message: "Initial website upload"
4. Click **Commit changes**

### Step 3: Enable GitHub Pages

1. Go to your repository **Settings**
2. Click **Pages** in the left sidebar
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**
6. Wait 1-2 minutes for deployment

### Step 4: Connect Custom Domain (Porkbun)

1. In GitHub Pages settings, enter your custom domain: `g6pdresearch.org`
2. Click **Save**

**In Porkbun DNS Settings:**

Add these DNS records:

| Type | Host | Answer |
|------|------|--------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR-USERNAME.github.io |

3. Wait 24-48 hours for DNS propagation
4. Check "Enforce HTTPS" in GitHub Pages settings once DNS is verified

---

## Website Features

### 1. Hero Section
- Interactive 3D protein visualization using PDBe Mol* viewer
- Key statistics about G6PD deficiency
- Smooth animations and modern design

### 2. About Section
- Personal G6PD journey and motivation
- Academic credentials and achievements
- Professional presentation of research goals

### 3. Research Library
- Top 20 most-cited G6PD research papers
- Citation counts and journal information
- Links to PubMed for further reading

### 4. AlphaFold Explorer
- Embedded 3D protein structure viewer
- Explanation of G6PD structure and function
- Interactive variant selection (Wild Type, Mediterranean, A-)

### 5. CRISPR Therapeutics
- Timeline of CRISPR development
- Proposed therapeutic strategy for G6PD
- Visual representation of gene correction approach

### 6. Community
- Newsletter signup form (via Formspree)
- Feedback/contact form
- Privacy-respecting implementation

### 7. Contact
- Email contact
- Links to G6PD.ai
- Location information

---

## Form Setup (Formspree)

The forms are already configured to work. However, you should:

1. Go to [formspree.io](https://formspree.io)
2. Create a free account
3. Create a new form
4. Copy your form endpoint (looks like `https://formspree.io/f/xxxxxxxx`)
5. Replace the placeholder endpoint in `index.html` (search for `formspree.io/f/xeoqgjkp`)

---

## Technologies Used

- **HTML5/CSS3** - Modern semantic markup and styling
- **PDBe Mol*** - 3D protein structure visualization
- **AlphaFold Database** - Protein structure predictions
- **Lucide Icons** - Clean, modern iconography
- **Formspree** - Form handling without backend
- **Google Fonts** - Inter, Playfair Display, JetBrains Mono

---

## Customization

### Changing Colors
Edit the CSS variables at the top of the `<style>` section:

```css
:root {
    --primary: #0066CC;        /* Main blue */
    --secondary: #10B981;      /* Green accent */
    --accent: #8B5CF6;         /* Purple accent */
}
```

### Adding Your Photo
Replace the placeholder in the About section with your actual photo:

```html
<div class="about-image">
    <img src="your-photo.jpg" alt="Luke Chen" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```

---

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (fully responsive)

---

## Credits

- **AlphaFold** by DeepMind
- **PDBe Mol*** by EMBL-EBI
- **Research papers** from PubMed/NCBI
- **Icons** from Lucide

---

## Contact

**Luke Chen**
Email: fight.g6pd.deficiency@gmail.com
Website: [www.g6pd.ai](https://www.g6pd.ai)

---

*Built with dedication to advancing G6PD deficiency research.*
