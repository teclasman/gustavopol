# gustavopol.com — Instrucciones

## Estructura de archivos

```
gustavopol/
├── index.html          ← Tu página web
├── netlify.toml        ← Configuración de Netlify
├── admin/
│   ├── index.html      ← Panel de administración
│   └── config.yml      ← Define qué puedes editar
└── _data/              ← (se crea automáticamente)
```

## Cómo subir el sitio a Netlify

1. Ve a https://github.com y crea una cuenta gratuita
2. Crea un repositorio nuevo llamado `gustavopol`
3. Sube todos estos archivos al repositorio
4. Ve a https://netlify.com, conéctalo con tu GitHub
5. Netlify detectará el proyecto y lo publicará solo

## Cómo activar el panel de edición (/admin)

En Netlify, una vez publicado:
1. Ve a **Site settings → Identity → Enable Identity**
2. Ve a **Identity → Services → Enable Git Gateway**
3. En **Identity → Registration**, pon "Invite only"
4. En **Identity → Invite users**, invítate con tu email
5. Recibirás un email → haz clic y crea tu contraseña

¡Listo! Ya puedes entrar a `gustavopol.com/admin` con tu email y contraseña.

## Cómo editar tu web (uso diario)

1. Ve a **gustavopol.com/admin**
2. Inicia sesión con tu email
3. Elige qué sección editar (Bio, Proyectos, Redes...)
4. Cambia lo que quieras
5. Haz clic en **Publicar**
6. En 30 segundos tu web se actualiza

## Conectar tu dominio de IONOS

1. En Netlify → **Domain settings → Add custom domain** → escribe `gustavopol.com`
2. Netlify te dará 4 nameservers (algo como `dns1.p01.nsone.net`)
3. Entra en IONOS → **Dominios → gustavopol.com → Nameservers**
4. Cambia los nameservers por los de Netlify
5. Espera 10–60 minutos → ¡tu dominio ya apunta a tu web!
6. Netlify activa HTTPS automáticamente (candado verde ✅)
