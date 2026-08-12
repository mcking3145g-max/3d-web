PREMIUM 3D FASHION STORE — GITHUB FRIENDLY VERSION

Start page:
- index.html

Pages:
- index.html
- tee-3d.html
- shirt-3d.html

Shirt 3D assets are now external instead of embedded inside shirt-3d.html:
- assets/shirt/scene.gltf
- assets/shirt/scene.bin
- assets/shirt/textures/*

This keeps shirt-3d.html very small and avoids GitHub's large single-file upload problem.

IMPORTANT:
Do not upload only shirt-3d.html by itself. Upload the whole folder structure so scene.gltf can find scene.bin and the textures.

Recommended GitHub structure:
/
  index.html
  tee-3d.html
  shirt-3d.html
  assets/
    shirt/
      scene.gltf
      scene.bin
      license.txt
      textures/
        ...

Deploy the repository to Vercel or GitHub Pages. The site should be served over HTTP/HTTPS rather than opened directly with file:// because GLTFLoader fetches the external model assets.
