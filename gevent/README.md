Online Version: http://sdiehl.github.com/gevent-tutorial/
=========================================================

Quieres agregar un ejemplo. Es súper simple.

1. Fork el repo.
2. ``pip install -r requirements.txt``
3. Editar ``tutorial.md``.

Agregar tu texto como Markdown.

Agregar tu código como Cog:

     [[[cog

     print("Hello World!")
     for i in xrange(25):
         print(i)

     ]]]
     [[[end]]]


Tendrás este output como html:

    <pre>
    <code class="python">

    print("Hello World!")
    for i in xrange(5):
        print(i)

    </code>
    </pre>

    <pre><code class="python">
    Hello World!
    0
    1
    2
    3
    4
    </code>
    </pre>

4. Ejecutar ``./build``
5. Solicitar pull request.
6. Obtener un buen karma gevent.

Liberado bajo Licencia MIT.

    Copyright (c) 2011 Stephen Diehl, <stephen.m.diehl@gmail.com>

    Permission is hereby granted, free of charge, to any person obtaining
    a copy of this software and associated documentation files (the
    "Software"), to deal in the Software without restriction, including
    without limitation the rights to use, copy, modify, merge, publish,
    distribute, sublicense, and/or sell copies of the Software, and to
    permit persons to whom the Software is furnished to do so, subject to
    the following conditions:

    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
    LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
    OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
    WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
