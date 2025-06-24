---
layout: default
title: Acerca de
permalink: /about/
---

<div class="py-5">
    <div class="container">
        <div class="row">
            <div class="col-lg-8 mx-auto">
                <div class="text-center mb-5">
                    <!-- <img src="{{ '/assets/img/profile.jpg' | relative_url }}" -->
                         <!-- alt="Foto de perfil" -->
                         <!-- style="max-width: 200px;"> -->
                    <h1 class="display-4 fw-bold">{{ site.title }}</h1>
                    <p class="lead text-muted">Desarrollador, Freelance, YouTuber, Docente y Escritor</p>
                </div>

                <div class="post-content">
                    <h2>¡Hola! 👋</h2>
                    
                    <p>Bienvenido a mi blog personal. Soy un apasionado de la tecnología y el desarrollo de software. Aquí comparto mis experiencias, aprendizajes y reflexiones sobre diversos topics relacionados con:</p>

                    <ul>
                        <li><strong>Desarrollo Web</strong>: Frontend, backend y arquitectura de aplicaciones</li>
                        <li><strong>Tecnología</strong>: Tendencias, tutoriales y análisis de nuevas herramientas</li>
                    </ul>

                    <h3>Mi trayectoria</h3>
                    
                    <p>Con más de X años de experiencia en el desarrollo de software y la investigación académica, he tenido la oportunidad de trabajar en diversos proyectos que van desde aplicaciones web hasta sistemas de análisis de datos complejos.</p>

                    <blockquote>
                        "La mejor manera de aprender es enseñando y compartiendo conocimiento con otros."
                    </blockquote>

                    <h3>Educación</h3>
                    
                    <ul>
                        <li><strong>Ingeniero en Sistemas Informáticos</strong> - Universidad de Oriente, El Salvador</li>
                    </ul>

                    <h3>Tecnologías que uso</h3>
                    
                    <div class="row mt-4">
                        <div class="col-md-6">
                            <h5>Frontend</h5>
                            <div class="mb-3">
                                <span class="badge bg-primary me-2">JavaScript</span>
                                <span class="badge bg-primary me-2">Vue.js</span>
                                <span class="badge bg-primary me-2">Bootstrap</span>
                                <span class="badge bg-primary me-2">TailwindCSS</span>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <h5>Backend</h5>
                            <div class="mb-3">
                                <span class="badge bg-success me-2">PHP</span>
                                <span class="badge bg-success me-2">Laravel</span>
                                <span class="badge bg-success me-2">C#</span>
                                <span class="badge bg-success me-2">ASP.NET</span>
                                <span class="badge bg-success me-2">Typescript</span>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <h5>Bases de Datos</h5>
                            <div class="mb-3">
                                <span class="badge bg-danger me-2">MySQL</span>
                                <span class="badge bg-danger me-2">SQL Server</span>
                                <span class="badge bg-danger me-2">MongoDB</span>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <h5>Herramientas</h5>
                            <div class="mb-3">
                                <span class="badge bg-secondary me-2">Git</span>
                                <span class="badge bg-secondary me-2">Docker</span>
                                <span class="badge bg-secondary me-2">GitHub</span>
                                <span class="badge bg-secondary me-2">Linux</span>
                            </div>
                        </div>
                    </div>

                    <h3>Contacto</h3>
                    
                    <p>Si tienes alguna pregunta, propuesta de colaboración o simplemente quieres conversar sobre tecnología e investigación, no dudes en contactarme:</p>

                    <div class="row mt-4">
                        <div class="col-md-6">
                            <div class="d-flex align-items-center mb-3">
                                <i class="bi bi-envelope-fill text-primary me-3" style="font-size: 1.5rem;"></i>
                                <div>
                                    <strong>Email</strong><br>
                                    <a href="mailto:{{ site.email }}">{{ site.email }}</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="d-flex align-items-center mb-3">
                                <i class="bi bi-github text-primary me-3" style="font-size: 1.5rem;"></i>
                                <div>
                                    <strong>GitHub</strong><br>
                                    <a href="https://github.com/{{ site.github_username }}" target="_blank">@{{ site.github_username }}</a>
                                </div>
                            </div>
                        </div>
                        <div class="col-md-6">
                            <div class="d-flex align-items-center mb-3">
                                <i class="bi bi-youtube text-primary me-3" style="font-size: 1.5rem;"></i>
                                <div>
                                    <strong>YouTube</strong><br>
                                    <a href="https://youtube.com/{{ site.youtube_username }}" target="_blank">{{ site.youtube_username }}</a>
                                </div>
                            </div>
                        </div>
                    </div>

                    <hr class="my-5">

                    <div class="text-center">
                        <p class="text-muted">
                            <em>"El conocimiento compartido es conocimiento multiplicado."</em>
                        </p>
                        <a href="{{ '/blog' | relative_url }}" class="btn btn-primary">
                            <i class="bi bi-arrow-left"></i> Volver al blog
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
