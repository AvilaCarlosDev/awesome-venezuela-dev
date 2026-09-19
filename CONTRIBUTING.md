# Contribuir / Contributing

[Español](#español) · [English](#english)

## Español

Gracias por querer sumar. La lista solo tiene valor si sus enlaces funcionan y sus recursos siguen activos.

### Qué se acepta

- Comunidades de desarrolladores venezolanos y de Venezuela.
- Recursos de aprendizaje gratuitos y en español.
- Información útil para trabajar en remoto desde Venezuela.
- Desarrolladores venezolanos (te puedes agregar tú mismo).

### Qué no se acepta

- Spam o autopromoción excesiva.
- Recursos inactivos o abandonados, o enlaces que no funcionan.
- Contenido sin relación con tecnología o sin relación con Venezuela.
- Enlaces de invitación a grupos privados: si un grupo debe enlazarse, que sea a su directorio público.

### Cómo proponer un cambio

1. Haz fork y crea una rama: `git checkout -b agrega-recurso`.
2. Edita `README.md` **y** `README.en.md`: las dos versiones deben enlazar exactamente lo mismo.
3. Sigue el formato de cada sección:
   - Recursos: `- **[Nombre](https://url)** — descripción corta`
   - Desarrolladores: una fila `| Nombre | Área | [@usuario](https://github.com/usuario) |`
4. Comprueba en local (opcional): `scripts/check-parity.sh README.md README.en.md` y `tests/check-parity.test.sh`.
5. Abre un Pull Request y completa la lista de verificación.

### Qué revisa el CI

- Que los enlaces respondan (lychee), cada semana y en cada cambio de un `.md`.
- Que `README.md` y `README.en.md` tengan los mismos enlaces.
- ShellCheck de los scripts, escaneo de secretos y ausencia de marcas de agua de IA.

La revisión final es humana y la hace una sola persona, sin plazo garantizado. El CI no puede juzgar si un recurso es bueno.

Si usaste un asistente de IA, menciónalo en la descripción del PR; el CI rechaza marcas de agua de IA en archivos y mensajes de commit.

## English

Thanks for wanting to help. The list is only valuable if its links work and its resources are still active.

### What is accepted

- Communities of Venezuelan developers and developers in Venezuela.
- Free learning resources, in Spanish.
- Useful information for working remotely from Venezuela.
- Venezuelan developers (you may add yourself).

### What is not accepted

- Spam or excessive self-promotion.
- Inactive or abandoned resources, or links that do not work.
- Content unrelated to technology or to Venezuela.
- Invite links to private groups: if a group must be linked, link to its public directory.

### How to propose a change

1. Fork and create a branch: `git checkout -b add-resource`.
2. Edit `README.md` **and** `README.en.md`: both versions must link exactly the same things.
3. Follow each section's format:
   - Resources: `- **[Name](https://url)** — short description`
   - Developers: a row `| Name | Area | [@user](https://github.com/user) |`
4. Check locally (optional): `scripts/check-parity.sh README.md README.en.md` and `tests/check-parity.test.sh`.
5. Open a Pull Request and complete the checklist.

### What CI checks

- That links respond (lychee), every week and on every change to a `.md` file.
- That `README.md` and `README.en.md` have the same links.
- ShellCheck for the scripts, secret scanning and absence of AI watermarks.

The final review is human and done by one person, with no guaranteed turnaround. CI cannot judge whether a resource is good.

If you used an AI assistant, say so in the PR description; CI rejects AI watermarks in files and commit messages.
