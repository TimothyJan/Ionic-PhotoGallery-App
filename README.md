# Ionic-PhotoGallery-App
Photo Gallery app that offers the ability to take photos with your device's camera, display them in a grid, and store them permanently on the device.

<a href="https://ionicframework.com/docs/angular/your-first-app">Tutorial</a>

Highlights include:
<ul>
  <li>One Angular-based codebase that runs on the web, iOS, and Android using Ionic Framework UI components.</li>
  <li>Deployed as a native iOS and Android mobile app using Capacitor, Ionic's official native app runtime.</li>
  <li>Photo Gallery functionality powered by the Capacitor Camera, Filesystem, and Preferences APIs.</li>
</ul>

Saving Photos to the Filesystem
<ul>
  <li>Using Capacitor <a href="https://capacitorjs.com/docs/apis/filesystem">Filesystem API</a> to save photo to the filesystem.</li>
  <li>Convert the photo to base64 format, then feed the data to the Filesystem’s writeFile function.</li>
</ul>

Loading Photos from the File system
<ul>
  <li>Leverage the Capacitor <a href="https://capacitorjs.com/docs/apis/preferences">Preferences API</a> to store our array of Photos in a key-value store.</li>
</ul>

Adding Mobile
<ul>
  <li>Import the Ionic <a href="https://ionicframework.com/docs/angular/platform">Platform API</a> into photo.service.ts, which is used to retrieve information about the current device.</li>
  <li>If it’s “hybrid” (Capacitor or Cordova, two native runtimes), then read the photo file into base64 format using the Filesystem readFile() method. Otherwise, Fetch the photo, read as a blob, then convert to base64 format.</li>
  <li></li>
</ul>
