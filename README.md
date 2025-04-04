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
Cloude name                ...
API key                    ...
API secret                 ...
API environment variable   ...
```

#### Visual Studio Code
Explorer
Open Editors
.env 

.env
```env
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=
NEXT_PUBLIC_CLOUDINARY_URL=
NEXT_PUBLIC_CLOUDINARY_API_SECRET=
NEXT_PUBLIC_CLOUDINARY_API_KEY=
```

#### Visual Studio Code
```
Explorer
Open Editors
.env 
.gitignore
```

.gitignore
```gitignore
.env
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/index.jsx
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "@/components/Header"

const Home = () => {
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <div></div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/index.jsx
pages/_document.jsx 
.env
.gitignore
```

pages/_document.jsx 
```javascript
import { Html, Head, Main, NextScript } from "next/document"

const Document = () => {
  return (
    <Html lang="en">
      <Head />
      <body>
        <Main />
        <NextScript />
      </body>
    </Html>
  )
}
export default Document
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/index.jsx
pages/_document.js 
pages/_app.jsx
.env
.gitignore
```

pages/_app.jsx
```javascript
import "@/styles/globals.css"

const App = ({ Component, pageProps }) => {
  return <Component {...pageProps} />
}
export default App
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/index.jsx
pages/_document.js 
pages/_app.jsx
styles/globals.css
.env
.gitignore
```

styles/globals.css
```css

```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
styles/globals.css
.env
.gitignore
```

pages/api/assets.js
```javascript

```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
styles/globals.css
.env
.gitignore
```

```

```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
styles/globals.css
.env
.gitignore
```

src/components/Dashboard.jsx
```javascript
const Dashboard = () => {
    return (
        <div>
            <h1>Dashboard</h1>
        </div> 
    )
}
export default Dashboard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
styles/globals.css
.env
.gitignore
```

src/componet/Header.jsx
```javascript   
const Header = () => {
    return (
        <div>
            <h1>Header</h1>
        </div> 
    )
}
export default Header
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/ImageCard.jsx
```javascript
const ImageCard = () => {
    return (
        <div>
            <h1>ImageCard</h1>
        </div> 
    )
}
export default ImageCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
styles/globals.css
.env
.gitignore
```

src/component/sideBar.jsx
```javascript
const sideBar = () => {
    return (
        <div>
            <h1>sideBar</h1>
        </div> 
    )
}
export default sideBar
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/VideoCard.jsx
```javascript
const VideoCard = () => {
    return (
        <div>
            <h1>VideoCard</h1>
        </div> 
    )
}
export default VideoCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/Header.jsx
```javascript   
import Image from "next/image"

const Header = () => {
    return (
        <div>
            <h1>Header</h1>
        </div> 
    )
}
export default Header
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"
import Header from "@/components/Header"

const Home = () => {
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header />
      <div></div> 
  )
}
export default Home
```

#### Visual Studio Code
Terminal
```     
npm run dev
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

public/drive_logo.png
```
Google Drive Logo ( Image )
```   

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/Header.jsx
```javascript   
import Image from "next/image"

const Header = () => {
    return (
        <header>
            <Image 
                src="/drive_logo.png"
                alt="Drive Logo"
                width={50}
                height={50}
            />
            <h1>Drive</h1>
        </header>
    )
}
export default Header
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

styles/globals.css
```css  
* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}
```

#### Google Fonts

> Poppins
- https://fonts.google.com/specimen/Poppins?query=poppins

1. Get embed code
2. Web
3. @import
4. Change styles
   - Light 300
   - Light 300 Italic

Embed code in the <head> of your html

5. Copy code
6. Past in the styles/globals.css file

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

styles/globals.css
```css  
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/components/Dashboard.jsx
```javascript
import ImageCard from "./ImageCard"
import VideoCard from "./VideoCard"

const Dashboard = () => {
    return (
        <main>
            <h2>Welcome to Drive AI</h2>
            <input 
                  className="main-search" 
                  placeholder>"Search in Drive"
                  value={}
            />
            <div className="upload-container">
                 <ImageCard />
                 <VideoCard />
        </main> 
    )
}
export default Dashboard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"

const Home = () => {
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header/>
      <div className="main-container">
        <Dashboard />
      </div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/ImageCard.jsx
```javascript
import { CldImage } from "next-cloudinary"

const ImageCard = () => {
    return (
        <article className="card">
            <div className="title-container">
               <h4><span className="emoji">ᝰ<span></span>{""}</h4>
               <h4>⫶</h4>
            </div>
            <CdlImage/>
            <div className="controls-container">
              <div className="controls-container">
                <input type="checkbox" id="background" name="background"/>
                <label htmlFor="background">no background</label>
              </div>

              <div className="controls-container">
                <input type="checkbox" id="greyscale" name="grayscale"/>
                <label htmlFor="greyscale">no background</label>
              </div>
            </div>

        </article>
    )
}
export default ImageCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}

.card {
  background-color: rgb(240, 244, 248);
  padding: 15px;
  border-radius: 15px; 
}

.title-container {
  display: flex;
  justify-content: space-between;
  width: 300px;
  height: 30px;
  overflow: hidden;
  margin: 20px 0;
}

.emoji {
  color:rgb(85, 85, 246);
}

.control-container {
  display: flex;
  padding: 3px 0 0 3px;
  height: 100%;
}

.control-container input[type="checkbox"] {
  margin: 3px;
  width: 10px;
}

.control-container label {
  margin-top: 2px;
}

.controls-container {
  display: flex;
  justify-content: space-between;
  height: 29px;
}

.controls-container, .controls-container button {
  font-size: 12px;
}

.card-input {
  width: 100%;
  height: 5px 0;
  box-sizing: border-box;
  padding: 3px;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/ImageCard.jsx
```javascript
import { CldImage } from "next-cloudinary"

const ImageCard = () => {
    return (
        <article className="card">
            <div className="title-container">
               <h4><span className="emoji">ᝰ<span></span>{""}</h4>
               <h4>⫶</h4>
            </div>
            <CdlImage/>
            <div className="controls-container">
              <div className="controls-container">
                <input type="checkbox" id="background" name="background"/>
                <label htmlFor="background">no background</label>
              </div>
              <div className="controls-container">
                <input type="checkbox" id="greyscale" name="grayscale"/>
                <label htmlFor="greyscale">no background</label>
              </div>
              <button>↓ download</button>
            </div>
            <input value={""} placeholder="Start typing to change image"/>

        </article>
    )
}
export default ImageCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/VideoCard.jsx
```javascript
import { CdlVideoPlayer } from "next-cloudinary"
import { useState } from "react"

const VideoCard = () => {
    const [isLoading, setIsLoading] = useState(true)

    return (
        <article className="card">
            <div className="title-container">
              <h4><span className="emoji">▶</span>{""}</h4>
              <h4>⫶</h4>
            </div>
            {isLoading && <p>Loading...</p>}

            <div className="video-container" 
                 style={{visibility: isLoading ? "hidden" : "visible"}}
            >
                {/*<CldVideoPlayer/> */} 
            </div>

            <div className="controls-container">
                 <div className="control-container">
                      <button>↓ download original</button>
                 </div>
            </div>
        </article>  
    )
}
export default VideoCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}

.card {
  background-color: rgb(240, 244, 248);
  padding: 15px;
  border-radius: 15px; 
}

.title-container {
  display: flex;
  justify-content: space-between;
  width: 300px;
  height: 30px;
  overflow: hidden;
  margin: 20px 0;
}

.emoji {
  color:rgb(85, 85, 246);
}

.control-container {
  display: flex;
  padding: 3px 0 0 3px;
  height: 100%;
}

.control-container input[type="checkbox"] {
  margin: 3px;
  width: 10px;
}

.control-container label {
  margin-top: 2px;
}

.controls-container {
  display: flex;
  justify-content: space-between;
  height: 29px;
}

.controls-container, .controls-container button {
  font-size: 12px;
}

.card-input {
  width: 100%;
  height: 5px 0;
  box-sizing: border-box;
  padding: 3px;
}

.video-container {
  margin-bottom: 5px;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/sideBar.jsx
```javascript
import { CldUploadWidget } from "next-cloudinary"

const sideBar = () => {
    return (
        <div>
            <article className="side-bar">
                {/*<CldUploadWidget/>*/}
                
                <ul>
                  <li>Home</li>
                  <li>Activity</li>
                  <li>Workspace</li>
                  <br/>
                  <li>My Drive</li>
                  <li>Shared Drives</li>
                  <br/>
                  <li>Shared with me</li>
                  <li>Recent</li>
                  <li>Starred</li>
                  <br/>
                  <li>Spam</li>
                  <li>Trash</li>
                  <li>Storage</li>
                </ul>
            
            </article>

        </div> 
    )
}
export default sideBar
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"
import Header from "@/components/Header"
import Dashboard from "@/components/Dashboard"
import sideBar from "@/components/sideBar" 

const Home = () => {
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header/>
      <div className="main-container">
        <sideBar/>
        <Dashboard/>
      </div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}

.card {
  background-color: rgb(240, 244, 248);
  padding: 15px;
  border-radius: 15px; 
}

.title-container {
  display: flex;
  justify-content: space-between;
  width: 300px;
  height: 30px;
  overflow: hidden;
  margin: 20px 0;
}

.emoji {
  color:rgb(85, 85, 246);
}

.control-container {
  display: flex;
  padding: 3px 0 0 3px;
  height: 100%;
}

.control-container input[type="checkbox"] {
  margin: 3px;
  width: 10px;
}

.control-container label {
  margin-top: 2px;
}

.controls-container {
  display: flex;
  justify-content: space-between;
  height: 29px;
}

.controls-container, .controls-container button {
  font-size: 12px;
}

.card-input {
  width: 100%;
  height: 5px 0;
  box-sizing: border-box;
  padding: 3px;
}

.video-container {
  margin-bottom: 5px;
}

.side-bar {
  width: 400px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: start;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/sideBar.jsx
```javascript
import { CldUploadWidget } from "next-cloudinary"

const sideBar = () => {
    return (
        <div>
            <article className="side-bar">
                <CldUploadWidget
                
                />
                
                <ul>
                  <li>Home</li>
                  <li>Activity</li>
                  <li>Workspace</li>
                  <br/>
                  <li>My Drive</li>
                  <li>Shared Drives</li>
                  <br/>
                  <li>Shared with me</li>
                  <li>Recent</li>
                  <li>Starred</li>
                  <br/>
                  <li>Spam</li>
                  <li>Trash</li>
                  <li>Storage</li>
                </ul>
            
            </article>

        </div> 
    )
}
export default sideBar
```

## Cloudinary UI

```
Settings

Product environment settings
  Upload
  Upload Presets  
    + Add Upload Preset
      Upload preset name
        demo_tutorial
      Signing mode
        Unsigned
      Asset folder
        dztmivw6w
          Save
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/sideBar.jsx
```javascript
import { CldUploadWidget } from "next-cloudinary"

const sideBar = () => {
    return (
        <div>
            <article className="side-bar">
                <CldUploadWidget
                  uploadPreset="demo_tutorial"
                  onSuccess={result => {
                    console.log(result)
                    onHandleNewUpload(result.info)
                  }}
                  onQueuesEnd={(result, { widget }) => {
                    widget.close()
                  }}
                >
                  {({ open}) => {
                    function handleOnClick() {
                      open()
                    }
                    return (
                      <button 
                          onClick={handleOnClick} 
                          className="new-button">+ New</button>
                    )
                  }}
                </CldUploadWidget>
                
                <ul>
                  <li>Home</li>
                  <li>Activity</li>
                  <li>Workspace</li>
                  <br/>
                  <li>My Drive</li>
                  <li>Shared Drives</li>
                  <br/>
                  <li>Shared with me</li>
                  <li>Recent</li>
                  <li>Starred</li>
                  <br/>
                  <li>Spam</li>
                  <li>Trash</li>
                  <li>Storage</li>
                </ul>
            
            </article>

        </div> 
    )
}
export default sideBar
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}

.card {
  background-color: rgb(240, 244, 248);
  padding: 15px;
  border-radius: 15px; 
}

.title-container {
  display: flex;
  justify-content: space-between;
  width: 300px;
  height: 30px;
  overflow: hidden;
  margin: 20px 0;
}

.emoji {
  color:rgb(85, 85, 246);
}

.control-container {
  display: flex;
  padding: 3px 0 0 3px;
  height: 100%;
}

.control-container input[type="checkbox"] {
  margin: 3px;
  width: 10px;
}

.control-container label {
  margin-top: 2px;
}

.controls-container {
  display: flex;
  justify-content: space-between;
  height: 29px;
}

.controls-container, .controls-container button {
  font-size: 12px;
}

.card-input {
  width: 100%;
  height: 5px 0;
  box-sizing: border-box;
  padding: 3px;
}

.video-container {
  margin-bottom: 5px;
}

.side-bar {
  width: 400px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: start;
}

.new-button {
  padding: 22px;
  margin: 10px 30px;
  border-radius: 15px;
  background-color: rgb(255, 255, 2550);
  border: none;
  font-size: 18px;
  box-shadow: rgba(50,50,50,93, 0.25) 0 2px 5px -1px, rgba(0,0,0,0.3) 0 1px 3px -1px;
}

.new-button:active {
  background-color: rgb(236, 238, 241);
  box-shadow: inset rgba(0,0,0,0.1), inset rgba(0,0,0,0.7) 0 -1px 0, 
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/sideBar.jsx
```javascript
import { CldUploadWidget } from "next-cloudinary"

const sideBar = ({onHandelNewUpload}) => {
    return (
        <div>
            <article className="side-bar">
                <CldUploadWidget
                  uploadPreset="demo_tutorial"
                  onSuccess={result => {
                    console.log(result)
                    onHandleNewUpload(result.info)
                  }}
                  onQueuesEnd={(result, { widget }) => {
                    widget.close()
                  }}
                >
                  {({ open}) => {
                    function handleOnClick() {
                      open()
                    }
                    return (
                      <button 
                          onClick={handleOnClick} 
                          className="new-button">+ New</button>
                    )
                  }}
                </CldUploadWidget>
                
                <ul>
                  <li>Home</li>
                  <li>Activity</li>
                  <li>Workspace</li>
                  <br/>
                  <li>My Drive</li>
                  <li>Shared Drives</li>
                  <br/>
                  <li>Shared with me</li>
                  <li>Recent</li>
                  <li>Starred</li>
                  <br/>
                  <li>Spam</li>
                  <li>Trash</li>
                  <li>Storage</li>
                </ul>
            
            </article>

        </div> 
    )
}
export default sideBar
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"
import { useState, useEffect } from "react"
import Header from "@/components/Header"
import Dashboard from "@/components/Dashboard"
import sideBar from "@/components/sideBar" 

const Home = () => {
  const [assets, setAssets] = useState([])
  
  const getData = async() => {
    try {
      const data = await fetch(`/api/assets`)
      const media = await data.json()
      setAssets(media)
    } catch (error) {
      console.log(error)
    }
  }

  useEffect(() => {
    getData()
  }, [])

  console.log(assets)

  const onHandleNewUpload = (asset) => {
    setAsset(prev => [asset, ...prev])
  }
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header/>
      <div className="main-container">
        <sideBar onHandleNewUpload={onHandleNewUpload}/>
        <Dashboard/>
      </div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/api/assets.js
```javascript
import { v2 as cloudinary } from "cloudinary"
```

#### Visual Studio Code
Terminal
```
npm i cloudinary
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/api/assets.js
```javascript
import { v2 as cloudinary } from "cloudinary"

cloudinary.config({
  cloud_name: process.env.NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME,
  api_key: process.env.NEXT_PUBLIC_CLOUDINARY_API_KEY,
  api_secret: process.env.NEXT_PUBLIC_CLOUDINARY_API_SECRET,
})

const handler = async (req, res) {
  const data = await cloudinary.search.execute()
  res.status(200).json(data.resources)
}

export default handler
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"
import { useState, useEffect } from "react"
import Header from "@/components/Header"
import Dashboard from "@/components/Dashboard"
import sideBar from "@/components/sideBar" 

const Home = () => {
  const [assets, setAssets] = useState([])
  
  const getData = async() => {
    try {
      const data = await fetch(`/api/assets`)
      const media = await data.json()
      setAssets(media)
    } catch (error) {
      console.log(error)
    }
  }

  useEffect(() => {
    getData()
  }, [])

  console.log(assets)

  const onHandleNewUpload = (asset) => {
    setAsset(prev => [asset, ...prev])
  }
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header/>
      <div className="main-container">
        <sideBar onHandleNewUpload={onHandleNewUpload}/>
        <Dashboard assets={assets}/>
      </div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/components/Dashboard.jsx
```javascript
import ImageCard from "./ImageCard"
import VideoCard from "./VideoCard"

const Dashboard = ({assets}) => {
    return (
        <main>
            <h2>Welcome to Drive AI</h2>
            <input 
                  className="main-search" 
                  placeholder>"Search in Drive"
                  value={}
            />
            <div className="upload-container">
                 {assets?.map(asset => 
                    asset.resource_type == "image" && 
                    <ImageCard key={asset.asset.id} asset={asset}/> 
                    || 
                    <VideCard key={asset.asset.id} asset={asset}/>
                 )}
                 <ImageCard />
                 <VideoCard />
            </div>
        </main> 
    )
}
export default Dashboard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/ImageCard.jsx
```javascript
import { CldImage } from "next-cloudinary"

const ImageCard = ({ asset }) => {
  const { public_id, display_name } = asset

    return (
        <article className="card">
            <div className="title-container">
               <h4><span className="emoji">ᝰ<span></span>{display_name}</h4>
               <h4>⫶</h4>
            </div>
            <CdlImage
              src={public_id}
              width="300"
              height="300"
              id={public_id}
              alt={display_name}
              crop={{
                type: "auto",
                source: "true",
              }}
            />
            <div className="controls-container">
              <div className="controls-container">
                <input type="checkbox" id="background" name="background"/>
                <label htmlFor="background">no background</label>
              </div>
              <div className="controls-container">
                <input type="checkbox" id="greyscale" name="grayscale"/>
                <label htmlFor="greyscale">no background</label>
              </div>
              <button>↓ download</button>
            </div>
            <input value={""} placeholder="Start typing to change image"/>

        </article>
    )
}
export default ImageCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/components/Dashboard.jsx
```javascript
import ImageCard from "./ImageCard"
import VideoCard from "./VideoCard"

const Dashboard = ({assets}) => {
    return (
        <main>
            <h2>Welcome to Drive AI</h2>
            <input 
                  className="main-search" 
                  placeholder>"Search in Drive"
                  value={}
            />
            <div className="upload-container">
                 {assets?.map(asset => 
                    asset.resource_type == "image" && 
                    <ImageCard key={asset.asset.id} asset={asset}/> 
                    || 
                    <VideCard key={asset.asset.id} asset={asset}/>
                 )}
            </div>
        </main> 
    )
}
export default Dashboard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

globals.css
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;1,300&display=swap');


* {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  color: rgb(40, 40, 40);
}

html, body {
  margin: 0;
  padding: 0;
}

h1 {
  padding: 0 0 0 10px;
  margin: 0;
}

h2 {
  padding: 20px;
  font-size: 28px;
}

h4 {
  font-size: 20px;
  margin: 0;
}

body {
  background-color: rgb(240, 244, 248);
}

header {
  padding: 20px 40px;
  display: flex;
  align-items: center;
}

.main-container {
  display: flex;
}

main {
  background-color: rgb(250, 250, 250);
  width: 100%;
  height: 100vh;
  boarder-radius: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  overflow-y: scroll;
}

.main-search {
  background-color: rgb(240, 244, 248);
  border: none;
  font-size: 20px;
  padding: 10px 30px;
  margin: 0 0 60px 0;
  border-radius: 30px;
  color: rgb(95, 99, 104);
  width: 60%;
}

.card {
  background-color: rgb(240, 244, 248);
  padding: 15px;
  border-radius: 15px; 
}

.title-container {
  display: flex;
  justify-content: space-between;
  width: 300px;
  height: 30px;
  overflow: hidden;
  margin: 20px 0;
}

.emoji {
  color:rgb(85, 85, 246);
  margin-right: 7px; 
}

.control-container {
  display: flex;
  padding: 3px 0 0 3px;
  height: 100%;
}

.control-container input[type="checkbox"] {
  margin: 3px;
  width: 10px;
}

.control-container label {
  margin-top: 2px;
}

.controls-container {
  display: flex;
  justify-content: space-between;
  height: 29px;
}

.controls-container, .controls-container button {
  font-size: 12px;
}

.card-input {
  width: 100%;
  height: 5px 0;
  box-sizing: border-box;
  padding: 3px;
}

.video-container {
  margin-bottom: 5px;
}

.side-bar {
  width: 400px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: start;
}

.new-button {
  padding: 22px;
  margin: 10px 30px;
  border-radius: 15px;
  background-color: rgb(255, 255, 2550);
  border: none;
  font-size: 18px;
  box-shadow: rgba(50,50,50,93, 0.25) 0 2px 5px -1px, rgba(0,0,0,0.3) 0 1px 3px -1px;
}

.new-button:active {
  background-color: rgb(236, 238, 241);
  box-shadow: inset rgba(0,0,0,0.1), inset rgba(0,0,0,0.7) 0 -1px 0, 
}

.uploads-container {
  width: 100%;
  display: grid;
  grid-template-columns: repeat(auto-fill, 330px);
  gap:20px;
  justify-content: center;
}

li {
  padding: 10px;
  font-size: 18px;
  list-style-type: none;
}
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/ImageCard.jsx
```javascript
import { CldImage } from "next-cloudinary"
import { useState } from "react"
import { saveAs } from "file-saver"
 
const ImageCard = ({ asset }) => {
  const { public_id, display_name } = asset

  const [ removeBackground, setRemoveBackground] = useState(false)
  const [ greyscale, setGreyscale] = useState(false)
  const [ prompt, setPrompt] = useState("")

  const downloadImage = () => {
    const imgSrc = document.getElementById(public_id).src
    saveAs(imgSrc, display_name)
  }

    return (
        <article className="card">
            <div className="title-container">
               <h4><span className="emoji">ᝰ<span></span>{display_name}</h4>
               <h4>⫶</h4>
            </div>
            <CdlImage
              src={public_id}
              width="300"
              height="300"
              id={public_id}
              alt={display_name}
              removeBackground={removeBackground}
              greyscale={greyscale}
              replaceBackground={prompt}
              crop={{
                type: "auto",
                source: "true",
              }}
            />
            <div className="controls-container">
              <div className="controls-container">
                <input type="checkbox" id="background" name="background" onChange={() => setRemoveBackground(!removeBackground)}/>
                <label htmlFor="background">no background</label>
              </div>
              <div className="controls-container">
                <input type="checkbox" id="greyscale" name="grayscale" onChange={() => setGreyscale(!greyscale)}/>
                <label htmlFor="greyscale">greyscale</label>
              </div>
              <button onClick={downloadImage}>↓ download</button>
            </div>
            <input value={prompt} placeholder="Start typing to change background" onChange={(e) => setPrompt(e.target.value)}/>

        </article>
    )
}
export default ImageCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/VideoCard.jsx
```javascript
import { CdlVideoPlayer } from "next-cloudinary"
import { useState, useEffect } from "react"
import { saveAS } from "file-saver"

const VideoCard = ({ asset }) => {
    const { public_id, display_name } = asset
    const [isLoading, setIsLoading] = useState(true)
    const [ retries, setRetries ] = useState(0)
    const [ errorOccurred, setErrorOccurred ] = useState(false)

    const downloadOGVideo = () => {
        const vidSrc = asset.url
        saveAs(vidSrc, display_name)
    }
 
    const handleVideoError = (err) => {
      if (err?.player?.videojs?.error_?.statusCode === 423 ) {
        if (!errorOccurred) {
          setErrorOccurred(true)
          setIsLoading(true)
          setRetries((prev) => prev + 1)
          console.log("Retrying video load...")
        }
      }
    }

    const handleMetaLoad = () => {
      setIsLoading(false)
      setErrorOccurred(false)
    }

    useEffect(() => {
      if (errorOccurred) {
        const intervalId = setInterval(() => {
          setRetries((prev) => prev + 1)
        }, 5000)

        return () => clearInterval(intervalId)

      }
    }, [errorOccurred])

    useEffect(() => {
      if (retries > 0 && !isLoading) {
        setIsLoading(false)
      }
    },[retries])

    return (
        <article className="card">
            <div className="title-container">
              <h4><span className="emoji">▶</span>{""}</h4>
              <h4>⫶</h4>
            </div>
            {isLoading && <p>Loading...</p>}

            <div className="video-container" 
                 style={{visibility: isLoading ? "hidden" : "visible"}}
            >
                <CldVideoPlayer 
                  src={public_id}
                  id={`${public_id}-${Math.random()}`}
                  height="300"
                  width="300"
                  alt={diplay_name}
                  transformation={{
                    width: "300",
                    height: "300",
                    crop: "fill",
                    gravity: "auto"
                  }}
                  onMetaLoad={handleMetaLoad}
                  onError={handleVideoError}
                />  
            </div>

            <div className="controls-container">
                 <div className="control-container">
                      <button onClick={downloadOGVideo}>↓ download original</button>
                 </div>
            </div>
        </article>  
    )
}
export default VideoCard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/index.jsx
```javascript
import Head from "next/head"
import { useState, useEffect } from "react"
import Header from "@/components/Header"
import Dashboard from "@/components/Dashboard"
import sideBar from "@/components/sideBar" 

const Home = () => {
  const [assets, setAssets] = useState([])
  const [searchTerm, setSearchTerm] = useState("")
  
  const getData = async() => {
    try {
      const data = await fetch(`/api/assets?${searchTerm}`)
      const media = await data.json()
      setAssets(media)
    } catch (error) {
      console.log(error)
    }
  }

  useEffect(() => {
    getData()
  }, [searchTerm])

  console.log(assets)

  const onHandleNewUpload = (asset) => {
    setAsset(prev => [asset, ...prev])
  }
  return (
    <>
      <Head>
        <title>Google Drive Clone</title>
        <meta name="description" content="Main page of Google Drive" />
        <meta name="viewport" content="width=device-width, initial-scale=1" />
      </Head>
      <Header/>
      <div className="main-container">
        <sideBar onHandleNewUpload={onHandleNewUpload}/>
        <Dashboard assets={assets} searchTerm={searchTerm} setSearchTerm={setSearchTerm}/>
      </div> 
  )
}
export default Home
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/components/Dashboard.jsx
```javascript
import ImageCard from "./ImageCard"
import VideoCard from "./VideoCard"

const Dashboard = ({assets, searchTerm, setSearchTerm}) => {
    return (
        <main>
            <h2>Welcome to Drive AI</h2>
            <input 
                  className="main-search" 
                  placeholder>"Search in Drive"
                  value={searchTerm}
                  onChange={(e) => setSearchTerm(e.target.value)}
            />
            <div className="upload-container">
                 {assets?.map(asset => 
                    asset.resource_type == "image" && 
                    <ImageCard key={asset.asset.id} asset={asset}/> 
                    || 
                    <VideCard key={asset.asset.id} asset={asset}/>
                 )}
            </div>
        </main> 
    )
}
export default Dashboard
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

pages/api/assets.js
```javascript
import { v2 as cloudinary } from "cloudinary"

cloudinary.config({
  cloud_name: process.env.NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME,
  api_key: process.env.NEXT_PUBLIC_CLOUDINARY_API_KEY,
  api_secret: process.env.NEXT_PUBLIC_CLOUDINARY_API_SECRET,
})

const handler = async (req, res) {
  const url = req.url.split("?")
  const searchTerm = url[1]
  const data = await cloudinary.search.expression(searchTerm).execute()
  res.status(200).json(data.resources)
}

export default handler
```

#### Visual Studio Code
```
Explorer
Open Editors
pages/api/assets.js
pages/index.jsx
pages/_document.js 
pages/_app.jsx
public/drive_logo.png
src/components/Dashboard.jsx
src/component/Header.jsx
src/component/ImageCard.jsx
src/component/sideBar.jsx
src/component/VideoCard.jsx
styles/globals.css
.env
.gitignore
```

src/component/VideoCard.jsx
```javascript
import { CdlVideoPlayer } from "next-cloudinary"
import { useState, useEffect } from "react"
import { saveAS } from "file-saver"

const VideoCard = ({ asset }) => {
    const { public_id, display_name } = asset
    const [isLoading, setIsLoading] = useState(true)
    const [ retries, setRetries ] = useState(0)
    const [ errorOccurred, setErrorOccurred ] = useState(false)

    const downloadOGVideo = () => {
        const vidSrc = asset.url
        saveAs(vidSrc, display_name)
    }
 
    const handleVideoError = (err) => {
      if (err?.player?.videojs?.error_?.statusCode === 423 ) {
        if (!errorOccurred) {
          setErrorOccurred(true)
          setIsLoading(true)
          setRetries((prev) => prev + 1)
          console.log("Retrying video load...")
        }
      }
    }

    const handleMetaLoad = () => {
      setIsLoading(false)
      setErrorOccurred(false)
    }

    useEffect(() => {
      if (errorOccurred) {
        const intervalId = setInterval(() => {
          setRetries((prev) => prev + 1)
        }, 5000)

        return () => clearInterval(intervalId)

      }
    }, [errorOccurred])

    useEffect(() => {
      if (retries > 0 && !isLoading) {
        setIsLoading(false)
      }
    },[retries])

    return (
        <article className="card">
            <div className="title-container">
              <h4><span className="emoji">▶</span>{display_name}</h4>
              <h4>⫶</h4>
            </div>
            {isLoading && <p>Loading...</p>}

            <div className="video-container" 
                 style={{visibility: isLoading ? "hidden" : "visible"}}
            >
                <CldVideoPlayer 
                  src={public_id}
                  id={public_id}
                  height="300"
                  width="300"
                  alt={diplay_name}
                  transformation={{
                    width: "300",
                    height: "300",
                    crop: "fill",
                    gravity: "auto"
                  }}
                  onMetaLoad={handleMetaLoad}
                  onError={handleVideoError}
                />  
            </div>

            <div className="controls-container">
                 <div className="control-container">
                      <button onClick={downloadOGVideo}>↓ download original</button>
                 </div>
            </div>
        </article>  
    )
}
export default VideoCard
```

