# Long Time Gone — website

Hiya Kellye. Your website is built with [Astro](https://astro.build). This README will hopefully explain how the project is organised and how to make common
edits yourself, but of course you can hit me up for help anytime.

---

## 1. Running the site on your computer

You only need to do this if you want to preview changes before they go
live.

1. Install [Node.js](https://nodejs.org) (LTS version) if you haven't already.
2. Open this project folder in your IDE's terminal.
3. Run once, the first time:
   ```bash
   npm install
   ```
4. Then, any time you want to preview the site:
   ```bash
   npm run dev
   ```
   This opens a local preview at `http://localhost:4321` that updates
   automatically as you edit and save files.

---

## 2. File structure

```
src/
├── layouts/
│   └── Layout.astro       
├── components/
│   ├── Contactform.astro
│   ├── Ctabanner.astro
│   ├── Header.astro        
│   ├── Hero.astro
│   ├── Imageband.astro
│   ├── Introheading.astro
│   ├── Textcontainer.astro
│   ├── Textimagesplit.astro  
│   └── Footer.astro         
├── pages/
│   ├── index.astro          
│   ├── about.astro    
│   ├── bespoke.astro     
│   ├── contact.astro
│   ├── blog.astro   
│   └── shop.astro   
└── styles/
    └── global.css         
public/
├── favicon-32x32.png
└── images/
```
Every page on the site is comprised of the Layout.astro file (which contains the site head information) and one or more components. I imagine you will probably get the most use out of the Textcontainer component, which is used for your 'About' and 'Bespoke' page, and basically just formats any text you write to look consistent.

A lot of these component files were thrown together really quickly by copy-pasting sections from the website scrape you provided me.

---

## 3. Editing existing pages

Just open the relevant file in `src/pages/` and edit the text directly
between the HTML tags. Blah blah blah, Yadda 

---

## 4. Styling (colours, fonts, layout)

All visual styling lives in `src/styles/global.css`. Components have their own styling, and these take precedence over styles in the global.css file.

All your colours and fonts live in global.

---

## 5. Images

Drop image files into `public/images/`. Anything placed there is
automatically available at `/images/your-file-name.jpg`.

I'd recommend switching out the .webp for higher resolution versions of your images at some point.

---

## 6. Publishing changes

I can't remember what was said about hosting these files, and i'm not 100% sure if we can use them as is or if we'll need to compile them. We'll find out soon enough!

---

## 7. To Do

Welcome to the suck...

- **Contact form** (`contact.astro`) — You'll need to connect this to your website via w3forms.com/
- **Shop page** (`shop.astro`) — This one is a bit rough at the moment, but I think it works alright! I'll pop some comments in at some point to help you make sense of it. The Layout.astro file has the head script which enables paypal.
- **Blog page** (`blog.astro`) — currently just embeds an Instagram feed widget, which is crap and only provides 200 unique views before it'll stop working. Will need to think on a long term replacement.
