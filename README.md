# responsive-video

## Responsive embed for the Vudoo iframe
Embedding your Vudoo video on your website? 
Tips and tricks to make your embedded Vudoo video look great on all devices and browser sizes.

**We'd recommend sending this page to your developer.**

Sometimes it can be hard to get embedded content to play nicely with the rest of your website's code. 
So, here's an example of how to embed a fluid responsive video that works seamlessly on your website.

Please note: 

These code examples are designed for use **on non-mobile devices** (eg. desktop computers, laptops, tablets). 
Vudoo videos are already optimised to play fullscreen and responsively on mobile devices.

### Fluid Responsive Video
Adding the Fluid Responsive code to your website will ensure your Vudoo video automatically adjusts its height and width depending on the viewer's device and/or browser. 

#### HTML Code Example
Add this HTML snippet within your website body tag. 

Please ensure you paste the appropriate Vudoo embed code within this snippet, replacing\
**"[PASTE VUDOO EMBED CODE HERE]"** entirely.

```html
<!-- VUDOO RESPONSIVE IFRAME HTML -->
<div class="vudoo--embed">
  <div class="video--outer">
    <div class="video--responsive video--ratio_16_9">
      <div class="video--wraper">

      [PASTE VUDOO EMBED CODE HERE]

      </div>
    </div>
  </div>
</div>
<!-- ./VUDOO RESPONSIVE IFRAME HTML -->
```


**CSS Code Example**\
Add this CSS code to your website styles file. 

```css
/**
 * VUDOO RESPONSIVE IFRAME CSS
 *
 */
.vudoo--embed {
	margin-right: auto;
	margin-left: auto;
	margin-top: 2em;
	margin-bottom: 2em;
	max-width: 1280px;
}

.vudoo--embed .video--outer {
	background-position: center center;
	background-size: cover;
	background-repeat: no-repeat;
}

.vudoo--embed .video--responsive {
	position: relative;
	width: 100%;
}

.vudoo--embed .video--ratio_16_9 {
	padding-top: 56.25%;
}

.vudoo--embed .video--wraper {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
}

.vudoo--embed iframe {
	width: 100%;
	height: 100%;
}
```

##### DISCLAIMER
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
