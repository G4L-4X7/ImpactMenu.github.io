<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Impact Menu</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html,
        body {
            width: 100%;
            min-height: 100%;
            font-family: Arial, sans-serif;
            overflow: hidden;
        }

        body {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #08090d;
            position: relative;
            isolation: isolate;
        }

        body::before {
            content: "";
            position: fixed;
            inset: -15px;
            background-image: url("https://cdn.discordapp.com/attachments/1565779631922094252/1566913889889951976/image.png?ex=6aea45c7&is=6ae8f447&hm=a6e4539f9f72a0d9fd224f7d427a5e698569945d114a8adac647306f2caeb57f&");
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            filter: blur(6px) brightness(0.65);
            transform: scale(1.02);
            z-index: -1;
        }

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 18px;
            width: 100%;
            padding: 24px;
        }

        .logo {
            display: block;
            width: min(420px, 80vw);
            height: auto;
            object-fit: contain;
            user-select: none;
            -webkit-user-drag: none;
        }

        .discord-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 52px;
            height: 52px;
            color: #5865F2;
            text-decoration: none;
            background: transparent;
            border: none;
            outline: none;
            transition: transform 0.25s ease;
        }

        .discord-icon {
            width: 34px;
            height: 34px;
            fill: currentColor;
            transition:
                color 0.25s ease,
                filter 0.25s ease,
                transform 0.25s ease;
        }

        .discord-link:hover .discord-icon {
            color: #7289ff;
            filter:
                drop-shadow(0 0 5px #5865F2)
                drop-shadow(0 0 12px #5865F2)
                drop-shadow(0 0 22px #386bff);
            transform: scale(1.13);
        }

        .discord-link:focus-visible {
            border-radius: 12px;
            outline: 2px solid #7289ff;
            outline-offset: 5px;
        }

        @media (max-width: 480px) {
            .logo {
                width: 85vw;
            }

            .container {
                gap: 14px;
            }
        }
    </style>
</head>
<body>
    <main class="container">
        <img class="logo" src="Impact Logo.png" alt="Impact Menu">

        <a
            class="discord-link"
            href="https://discord.gg/UHz5JRKsbe"
            target="_blank"
            rel="noopener noreferrer"
            aria-label="Join the Impact Discord server"
        >
            <svg class="discord-icon" viewBox="0 0 127.14 96.36" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
                <path d="M107.7 8.07A105.15 105.15 0 0 0 81.47 0a72.06 72.06 0 0 0-3.36 6.83 97.68 97.68 0 0 0-29.1 0A72.37 72.37 0 0 0 45.65 0a105.89 105.89 0 0 0-26.25 8.09C2.79 32.65-1.71 56.6.54 80.21A105.73 105.73 0 0 0 32.7 96.36a77.7 77.7 0 0 0 6.89-11.15 68.42 68.42 0 0 1-10.85-5.18c.91-.66 1.8-1.34 2.66-2.03a75.76 75.76 0 0 0 64.32 0c.87.71 1.76 1.39 2.66 2.03a68.68 68.68 0 0 1-10.87 5.19 77 77 0 0 0 6.89 11.14 105.25 105.25 0 0 0 32.17-16.13c2.64-27.38-4.52-51.11-18.87-72.16ZM42.45 65.69c-6.27 0-11.44-5.74-11.44-12.8s5.04-12.8 11.44-12.8 11.55 5.79 11.44 12.8c0 7.06-5.04 12.8-11.44 12.8Zm42.24 0c-6.27 0-11.44-5.74-11.44-12.8s5.04-12.8 11.44-12.8 11.55 5.79 11.44 12.8c0 7.06-5.04 12.8-11.44 12.8Z"/>
            </svg>
        </a>
    </main>
</body>
</html>

