# SMR2-SOR
```mermaid
graph TD;
A[Tareas]-->B[Hardware-Win10];
A-->C[Modo Dios];
A-->D[balenaEtcher];
A-->E[WSL];
A-->F[Docker Desktop];
B-->|Entras en la carpeta de Modo Dios| G[Buscas en el Administrador de dispositivos];
G-->|Entras en el Administrador de dispositivos| H[Ves para qué parte del hardware no hay drivers];
H-->|Buscas los drivers compatibles con el modelo de tu BIOS en Google| I[Instalas los drivers más recientes];
C-->|Creas una carpeta nueva en el escritorio| J[Le pones un comano como nombre, este comando está en aules];
D-->|Entras en https://portal.edu.gva.es/appsedu/balenaetcher/| K[Instalas la imagen ISO de balenaEtcher];
K-->|Ejecutas el balenaEtcher| L[Ya puedes hacer ejecutables en un dispositivo extraíble]
E-->|Entras en la página web de microsoft para aprender a instalar WSL en Windows| M[Abres el Windows PoweShell]
M-->|Buscas el comando que necesitas para instalar WSL| N[Ejecutas el comando en el Windows PowerShell]
F-->|Entras en https://portal.edu.gva.es/appsedu/docker-3/| O[Instalas la imagen ISO del Docker Desktop]
O-->|Creas una nueva cuenta de gmail| P[Ejecutas el Docker Desktop y creas una cuenta con el correo que acabas de crear]
