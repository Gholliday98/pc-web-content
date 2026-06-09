# Blog Post Template (v2) — Usage Guide

Matches the design at plastic-craft.com/n/ with a composed header (title + image side by side).

## How to Use

1. Open `base-blog-post.html` or have Claude generate a new post based on it
2. Replace everything between `CONTENT START` and `CONTENT END` with your actual content
3. In WordPress, add an **Elementor HTML widget** (or WP Custom HTML block)
4. Paste the entire HTML block
5. Publish

## Available Components

### Breadcrumb

```html
<nav class="pc-breadcrumb">
  <a href="https://plastic-craft.com">Plastic-Craft Products</a>
  <span class="pc-sep">&#8250;</span>
  <a href="https://plastic-craft.com/blog/">Industry Insights</a>
  <span class="pc-sep">&#8250;</span>
  <span>Post Title</span>
</nav>
```

### Header Block (title + image composed together)

```html
<div class="pc-header">
  <div class="pc-header-text">
    <span class="pc-category-tag">Category Name</span>
    <h1 class="pc-title">Post Title Goes Here</h1>
    <p class="pc-excerpt">Summary sentence here.</p>
    <div class="pc-post-meta">
      <span>March 16, 2026</span>
      <span>|</span>
      <span>Plastic-Craft Products</span>
    </div>
  </div>
  <img class="pc-header-img" src="YOUR_IMAGE_URL" alt="Alt text">
</div>
```

Title text on the left, image on the right, light gray background band ties them together. Stacks vertically on mobile. The image spot shows a dashed-border placeholder by default -- swap it the same way as all images (see "Image with Caption" below).

### Section Heading (H2 with chevron + underline)

```html
<h2>Section Heading Text</h2>
```

The navy chevron arrow and bottom border are automatic via CSS.

### Callout Box

```html
<div class="pc-callout">
  <p><strong>Key Takeaway:</strong> Your important note here.</p>
</div>
```

### Data Table

```html
<div class="pc-table-wrap">
  <table>
    <thead>
      <tr>
        <th>Column 1</th>
        <th>Column 2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Data</td>
        <td>Data</td>
      </tr>
    </tbody>
  </table>
</div>
```

### Three-Column Badge Row

```html
<div class="pc-badges">
  <div class="pc-badge">
    <div class="pc-badge-icon">
      <svg viewBox="0 0 24 24"><path d="..."/></svg>
    </div>
    <span class="pc-badge-label">Label Text</span>
  </div>
  <!-- repeat for 2nd and 3rd badge -->
</div>
```

### Gold Bullet List

```html
<ul class="pc-features">
  <li>Point one</li>
  <li>Point two</li>
</ul>
```

### Two-Column Layout

```html
<div class="pc-columns">
  <div>
    <h4>Left Heading</h4>
    <p>Left content.</p>
  </div>
  <div>
    <h4>Right Heading</h4>
    <p>Right content.</p>
  </div>
</div>
```

### Image Upload Zones

Every image spot is a clickable upload area. No code editing needed.

**How it works:**
1. Click the dashed placeholder area (or drag and drop a file onto it)
2. Pick your image
3. It appears instantly in the correct spot, styled and cropped automatically

The upload zones work in both the header and anywhere in the post body.

```html
<div class="pc-img-upload" style="aspect-ratio: 16 / 9;" onclick="this.querySelector('input').click()">
  <input type="file" accept="image/*" onchange="pcHandleUpload(this)">
  <label class="pc-upload-label">
    <svg viewBox="0 0 24 24"><path d="..."/></svg>
    <span>Click to Upload Image</span>
    <small>Or drag and drop your file here</small>
  </label>
  <img class="pc-uploaded-img" alt="Alt text">
</div>
```

Change the `aspect-ratio` to control shape: `4 / 3` for header, `16 / 9` for body images, etc.

### Navy CTA Banner

```html
<div class="pc-cta-banner">
  <h3>We're Always Open to the Conversation</h3>
  <p>Supporting text goes here.</p>
  <a href="tel:8453583010" class="pc-phone">(845) 358-3010</a>
</div>
```

### Inline CTA Button (gold)

```html
<a href="https://plastic-craft.com/contact/" class="pc-cta-btn">Request a Quote</a>
```

### Blockquote

```html
<blockquote>
  <p>Your quote or emphasis text here.</p>
</blockquote>
```

## Design Notes

- All styles scoped under `.pc-post` — no theme conflicts
- H2 headings automatically get the navy chevron icon and bottom border
- Fully responsive — columns and badges stack on mobile
- Fonts load from Google Fonts (Montserrat + Lora)
- No emojis, ever
- Every post should end with the navy CTA banner
- Header image sits beside the title in a composed block — not a full-width banner on top
- All image spots are click-to-upload — no code editing needed for images
