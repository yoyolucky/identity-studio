# Identity Studio Free — static web app

This is a real mobile-friendly web application, not a paid API integration. It lets you upload, locally store, delete and export identity photos and captions as a ZIP; record trained LoRA metadata; draft generation prompts; and save finished images in a local gallery.

## Open on iPhone for $0
Publish `index.html` and `manifest.webmanifest` using a free static host such as GitHub Pages or Cloudflare Pages. Use HTTPS for reliable local browser storage. On Safari, choose Share > Add to Home Screen. No server, account, subscription, or credit card is needed for this app. JSZip is loaded from a public CDN for ZIP export, so export requires network access.

## Real LoRA training
Use the exported ZIP with https://github.com/ostris/ai-toolkit on a GPU you have permission to use. Kaggle/Colab free-tier GPUs may be unavailable, too small or restricted by platform policies. There is **no guaranteed free automatic cloud training**. After training, download the `.safetensors` LoRA and retain its compatible base model information.

## Generation
Use https://github.com/comfyanonymous/ComfyUI with the same base-model family and your LoRA on a suitable GPU. iPhone local inference for large diffusion models is not implemented or realistically supported by this app. Import separately generated image files into the gallery.

## Privacy and limitations
Photos are stored in the browser's IndexedDB, not uploaded to a server. Clearing site data can erase them. This is a personal prototype; not a substitute for secure backup. No fake progress bars, GPU claims or pretend generated photos. The app is **not yet** an automated LoRA trainer or generator.
