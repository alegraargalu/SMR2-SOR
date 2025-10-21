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
