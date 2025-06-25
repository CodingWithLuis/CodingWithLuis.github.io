---
layout: posts
title: "Laravel: Encriptar variables de entorno"
date: 2025-06-23 10:00:00 -0600
categories: [tecnología, web]
tags: [Laravel, cifrado]
author: "Luis Zelaya"
reading_time: 5
---

Laravel a partir de la versión **9.32** introdujo dos nuevos comandos: **env:encrypt** y **env:decrypt**

Gracias a estos comandos ahora podemos guardar de manera segura una copia de nuestro archivo **.env** en nuestro entorno de control de versiones (GitHub, Gitlab o Bitbucket).

Si nosotros hacemos ese proceso vamos a contar con algunas ventajas como:

- Compartir el entorno de desarrollo entre diferentes miembros del equipo
- Desencriptar y cargar archivos de configuración de variables de entorno como parte del proceso de despligue
- Actualizar automáticamente entornos CI

## Comando env:encrypt

El comando **env:encrypt** lee un archivo de variables de entorno (.env) y encripta su contenido. Una vez encriptado el contenido se genera un nuevo archivo de variables de entorno con el sufijo **.encrypted**.

Para usar el comando debes ejecutar:

<div class="code-section">
    <div class="feedback-message" id="feedback">Copiado!</div>
        <button class="copy-button" onclick="copyCode()" id="copyBtn">
            <svg class="copy-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect>
                <path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path>
            </svg>
            Copiar
        </button>
    <pre class="code-content" id="codeContent">php artisan env:encrypt</pre>
</div>

## Comando env:decrypt

Para usar el comando debes ejecutar:

<div class="code-section">
    <div class="feedback-message" id="feedback">Copiado!</div>
        <button class="copy-button" onclick="copyCode()" id="copyBtn">
            <svg class="copy-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect>
                <path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path>
            </svg>
            Copiar
        </button>
    <pre class="code-content" id="codeContent">php artisan env:decrypt</pre>
</div>

   <script>
        function copyCode() {
            const codeContent = document.getElementById('codeContent').textContent;
            const copyBtn = document.getElementById('copyBtn');
            const feedback = document.getElementById('feedback');

            navigator.clipboard.writeText(codeContent).then(() => {
                // Update button appearance
                copyBtn.classList.add('copied');
                copyBtn.innerHTML = `
                    <svg class="copy-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <polyline points="20,6 9,17 4,12"></polyline>
                    </svg>
                    Copied!
                `;

                // Show feedback message
                feedback.classList.add('show');

                // Reset after 2 seconds
                setTimeout(() => {
                    copyBtn.classList.remove('copied');
                    copyBtn.innerHTML = `
                        <svg class="copy-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <rect x="9" y="9" width="13" height="13" rx="2" ry="2"></rect>
                            <path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"></path>
                        </svg>
                        Copy
                    `;
                    feedback.classList.remove('show');
                }, 2000);
            }).catch(err => {
                console.error('Failed to copy: ', err);

                // Fallback for older browsers
                const textArea = document.createElement('textarea');
                textArea.value = codeContent;
                document.body.appendChild(textArea);
                textArea.select();
                document.execCommand('copy');
                document.body.removeChild(textArea);

                feedback.textContent = 'Copied!';
                feedback.classList.add('show');
                setTimeout(() => {
                    feedback.classList.remove('show');
                }, 2000);
            });
        }
    </script>
