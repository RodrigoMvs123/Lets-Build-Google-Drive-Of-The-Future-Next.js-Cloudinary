#### Let's build Google Drive of the future!! Next.js Cloudinary

- https://www.youtube.com/watch?v=v5GE4OUNwXs 

1. A polished interface for file uploads, previews, and management
2. A drag-and-drop feature for seamless upload of pictures and videos
3. Integration with Cloudinary
4. A robust backend built with Next.js
5. AI removal of backgrounds on images
6. Greyscale on images
7. AI background on images
8. Ability to download manipulated images in-app
9. The ability to crop videos thanks to AI features

#### Visual Studio Code
Terminal
```
npx create-next-app@latest nextjs-google-drive

>   Would you like to use TypeScript with this project? › No 
    Would you like to use ESLint with this project? › Yes
    Would you like to use Tailwind CSS with this project? › Yes
    Would you like to use `src/` directory with this project? › Yes
    Would you like to use the App Router? (recommended) › No
    Would you like to use TurboPack for `next dev`? No
    Would you like to customize the default import alias? › No
```

#### Cloudinary 

- https://cloudinary.com/ip/codewithania 

Next.js

#### Visual Studio Code
Terminal
```
npm i next-cloudinary
```

#### Cloudinary

View API Keys
```
Cloude name                dztmivw6w
API key                    ...
API secret                 ...
API environment variable   CLOUDINARY_URL=cloudinary://358427952998453:Kr91h5mVbzJ25ZL-LSPUN2WcM44@dztmivw6w
```

#### Visual Studio Code
Explorer
Open Editors
.env 

.env
```env
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=dztmivw6w
NEXT_PUBLIC_CLOUDINARY_URL=CLOUDINARY_URL=CLOUDINARY_URL=CLOUDINARY_URL=cloudinary://358427952998453:Kr91h5mVbzJ25ZL-LSPUN2WcM44@dztmivw6w
NEXT_PUBLIC_CLOUDINARY_API_SECRET=
NEXT_PUBLIC_CLOUDINARY_API_KEY=
```

#### Visual Studio Code
Explorer
Open Editors
.env 
.gitignore

.gitignore
```gitignore
.env
```


