# HTML vs The DOM

<p>Looking at the HTML in the browser you'll see it is different to what is in the index.html file where the HTML contains an <i>h1</i> tag, where it does not exist in the index.html file. The <i>h1</i> tag exists only by the Javascript updating the DOM when the page is loaded.</p>


```
<html>
    <body>
        <div id="app"></div>

        <script type="text/javascript">

                const app = document.getElementById('app');
                const header = document.createElement('h1');

                const text = 'Develop. Preview. Ship';

                const headerContent = document.createTextNode(text);

                header.appendChild(headerContent);

                app.appendChild(header);
        </script>

    </body>
</html>

```