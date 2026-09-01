<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Contacto</title>
    <style>
    @media (max-width: 768px) {
        nav {
            flex-direction: column;
        }
    }
    
        :root {
            --bg: #f4f7fb;
            --card: #ffffff;
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --text: #1f2937;
            --muted: #6b7280;
            --border: #dbe3f0;
            --shadow: 0 20px 45px rgba(37, 99, 235, 0.12);
        }

        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            min-height: 100vh;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #edf4ff 0%, #f9fafb 100%);
            color: var(--text);
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 32px 20px;
        }

        .container {
            width: min(1100px, 100%);
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(219, 227, 240, 0.9);
            border-radius: 24px;
            box-shadow: var(--shadow);
            overflow: hidden;
        }

        .content {
            display: grid;
            grid-template-columns: 1fr 1.2fr;
        }

        .sidebar {
            background: linear-gradient(180deg, #0f172a 0%, #1e3a8a 100%);
            color: #fff;
            padding: 42px 32px;
        }

        .eyebrow {
            display: inline-block;
            font-size: 12px;
            letter-spacing: 0.12em;
            text-transform: uppercase;
            background: rgba(255, 255, 255, 0.12);
            padding: 8px 12px;
            border-radius: 999px;
            margin-bottom: 20px;
        }

        h1 {
            margin: 0 0 14px;
            font-size: clamp(2rem, 3vw, 3rem);
            line-height: 1.1;
        }

        .subtitle {
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.7;
            margin: 0 0 28px;
        }

        .contacts {
            display: grid;
            gap: 18px;
            margin-top: 24px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 14px;
            background: rgba(255, 255, 255, 0.08);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 16px;
            padding: 14px 16px;
        }

        .icon {
            width: 42px;
            height: 42px;
            border-radius: 12px;
            background: rgba(255, 255, 255, 0.15);
            display: grid;
            place-items: center;
            font-weight: bold;
            font-size: 1.1rem;
        }

        .contact-item p {
            margin: 0;
            font-size: 0.98rem;
            color: rgba(255, 255, 255, 0.9);
        }

        .photo-card {
            margin-top: 32px;
            background: rgba(148, 163, 184, 0.18);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 18px;
        }

        .photo-card img {
            display: block;
            width: 100%;
            max-width: 220px;
            height: 180px;
            object-fit: cover;
            border-radius: 16px;
            margin: 0 auto;
            box-shadow: 0 16px 30px rgba(15, 23, 42, 0.25);
        }

        .form-panel {
            background: var(--card);
            padding: 42px 32px;
        }

        .form-panel h2 {
            margin: 0 0 12px;
            font-size: 1.8rem;
        }

        .form-panel p {
            margin: 0 0 24px;
            color: var(--muted);
            line-height: 1.6;
        }

        form {
            display: grid;
            gap: 18px;
        }

        .field {
            display: grid;
            gap: 8px;
        }

        label {
            font-weight: 700;
            color: var(--text);
        }

        input, textarea {
            width: 100%;
            padding: 14px 16px;
            border: 1px solid var(--border);
            border-radius: 12px;
            background: #f8fafc;
            font-size: 1rem;
            transition: border-color 0.2s ease, box-shadow 0.2s ease, transform 0.2s ease;
        }

        input:focus, textarea:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.12);
            background: #fff;
        }

        textarea {
            min-height: 140px;
            resize: vertical;
        }

        button {
            border: none;
            border-radius: 12px;
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: white;
            font-size: 1rem;
            font-weight: 700;
            padding: 16px 22px;
            cursor: pointer;
            transition: transform 0.2s ease, box-shadow 0.2s ease;
            box-shadow: 0 12px 28px rgba(37, 99, 235, 0.25);
        }

        button:hover {
            transform: translateY(-1px);
            box-shadow: 0 16px 30px rgba(37, 99, 235, 0.3);
        }

        @media (max-width: 820px) {
            .content {
                grid-template-columns: 1fr;
            }

            .sidebar, .form-panel {
                padding: 28px 22px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="content">
            <aside class="sidebar">
                <span class="eyebrow">Contactar</span>
                <h1>Pues esto sirve para contactarme no?O_O</h1>
                <p class="subtitle">Si tienes algun problema o duda, estoy aqui para ayudarte</p>

                <div class="contacts">
                    <div class="contact-item">
                        <div class="icon">📞</div>
                        <p>+56 9 1234 5678</p>
                    </div>
                    <div class="contact-item">
                        <div class="icon">📨</div>
                        <p>d.de.go.r.p.t@gmail.com</p>
                    </div>
                </div>

                <div class="photo-card">
                    <img src="C:\Users\Alumno\Desktop\4-H\images.jpg" alt="Foto de contacto">
                </div>
            </aside>

            <section class="form-panel">
                <h2>Envíanos un mensaje</h2>
                <p>Completa este formulario y te responderemos (o tal vez no)</p>

                <form>
                    <div class="field">
                        <label for="nombre">Nombre de usuario</label>
                        <input type="text" id="nombre" name="nombre" placeholder="Tu nombre de usuario" required>
                    </div>

                    <div class="field">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email" placeholder="tuemail@ejemplo.com" required>
                    </div>

                    <div class="field">
                        <label for="mensaje">Mensaje</label>
                        <textarea id="mensaje" name="mensaje" placeholder="Escribe tu mensaje aquí..." required></textarea>
                    </div>

                    <button type="submit">Enviar mensaje</button>
                </form>
            </section>
        </div>
    </div>
</body>
</html>
