<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Comandos FIND, PS y GREP</title>
    <style>
        body { font-family: Arial, sans-serif; line-height: 1.6; margin: 40px; background-color: #f4f4f9; }
        .nav { margin-bottom: 20px; }
        .comando-section { background: #fff; padding: 20px; margin-bottom: 40px; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); }
        h1 { color: #333; border-bottom: 3px solid #0056b3; padding-bottom: 10px; }
        h2 { color: #0056b3; border-bottom: 1px solid #ccc; padding-bottom: 5px;}
        h3 { color: #204060; }
        .descripcion { background: #e9f2fa; padding: 15px; border-left: 4px solid #0056b3; margin-bottom: 15px; }
        code { background: #eee; padding: 2px 6px; border-radius: 4px; color: #d63384; font-weight: bold; font-family: monospace; }
        a { text-decoration: none; color: #0056b3; font-weight: bold; margin-right: 15px; }
        a:hover { text-decoration: underline; }
    </style>
</head>
<body>

    <div class="nav">
        <a href="README.md">← Volver al Índice</a>
        <a href="#find">Ir a FIND</a>
        <a href="#ps">Ir a PS</a>
        <a href="#grep">Ir a GREP</a>
    </div>

    <h1>Manual de Comandos Linux (Parte 1)</h1>

    <section id="find" class="comando-section">
        <h2>1. Comando FIND</h2>
        <div class="descripcion">
            <p>El comando <code>find</code> se utiliza en Linux para buscar archivos y directorios basándose en criterios como el nombre, tamaño, permisos o fecha de modificación.</p>
        </div>
        <div class="opciones">
            <h3>Opciones Principales</h3>
            <ul>
                <li><code>-name</code>: Busca archivos por su nombre exacto.</li>
                <li><code>-perm</code>: Busca archivos basándose en sus permisos octales.</li>
                <li><code>-size</code>: Busca archivos por su tamaño.</li>
            </ul>
        </div>
        <div class="ejemplos">
            <h3>Ejemplos de Uso</h3>
            <ul>
                <li>Buscar un archivo por nombre: <code>find / -name "documento.txt"</code></li>
                <li>Buscar archivos por permisos: <code>find . -perm 777</code></li>
            </ul>
        </div>
    </section>

    <section id="ps" class="comando-section">
        <h2>2. Comando PS</h2>
        <div class="descripcion">
            <p>El comando <code>ps</code> muestra una instantánea de los procesos que se están ejecutando actualmente en el sistema.</p>
        </div>
        <div class="opciones">
            <h3>Opciones Principales</h3>
            <ul>
                <li><code>-e</code>: Selecciona y muestra todos los procesos del sistema.</li>
                <li><code>-u</code>: Muestra los procesos correspondientes a un usuario.</li>
                <li><code>aux</code>: Muestra todos los procesos con información muy detallada.</li>
            </ul>
        </div>
        <div class="ejemplos">
            <h3>Ejemplos de Uso</h3>
            <ul>
                <li>Ver todos los procesos: <code>ps aux</code></li>
                <li>Buscar procesos de un usuario: <code>ps -u root</code></li>
            </ul>
        </div>
    </section>

    <section id="grep" class="comando-section">
        <h2>3. Comando GREP</h2>
        <div class="descripcion">
            <p>El comando <code>grep</code> se utiliza para buscar cadenas de texto o patrones dentro de uno o varios archivos.</p>
        </div>
        <div class="opciones">
            <h3>Opciones Principales</h3>
            <ul>
                <li><code>-i</code>: Ignora la distinción entre mayúsculas y minúsculas.</li>
                <li><code>-v</code>: Invierte la búsqueda (muestra lo que NO coincide).</li>
                <li><code>-r</code>: Búsqueda recursiva en subdirectorios.</li>
            </ul>
        </div>
        <div class="ejemplos">
            <h3>Ejemplos de Uso</h3>
            <ul>
                <li>Buscar una palabra en un archivo: <code>grep "error" log.txt</code></li>
                <li>Buscar en un proyecto entero: <code>grep -r "main" /carpeta/</code></li>
            </ul>
        </div>
    </section>

</body>
</html>