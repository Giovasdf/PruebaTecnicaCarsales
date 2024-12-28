# Rick and Morty BFF and App

Este proyecto implementa una arquitectura **Backend for Frontend (BFF)** para consumir la API pública de Rick and Morty y mostrar episodios en un frontend desarrollado con Angular. El BFF se encarga de intermediar entre el frontend y la API externa, simplificando la comunicación y mejorando la seguridad.

## **Estructura del Proyecto**

El proyecto está dividido en dos repositorios principales:

1. [RickAndMortyAPI (BFF)](https://github.com/Giovasdf/RickAndMortyAPI): Implementa la lógica del BFF utilizando .NET 8.
2. [RickAndMortyApp (Frontend)](https://github.com/Giovasdf/RickAndMortyApp): Aplicación de frontend creada con Angular 19 y utilizando standalone components.

---

## **Cómo Correr el Proyecto**

### **1. Backend (RickAndMortyAPI)**

#### **Requisitos**
- .NET 8 SDK instalado.

#### **Instrucciones**
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Giovasdf/RickAndMortyAPI
   cd RickAndMortyAPI
   cd RickAndMortyBFF
   ```

2. Restaura las dependencias:
   ```bash
   dotnet restore
   ```

3. Ejecuta el servidor:
   ```bash
   dotnet run
   ```

4. El servidor estará disponible en:
   - **HTTP**: `http://localhost:5247`
   - **HTTPS**: `https://localhost:7247`

---

### **2. Frontend (RickAndMortyApp)**

#### **Requisitos**
- Node.js (versión 18 o superior).
- Angular CLI instalado globalmente:
   ```bash
   npm install -g @angular/cli
   ```

#### **Instrucciones**
1. Clona el repositorio:
   ```bash
   git clone https://github.com/Giovasdf/RickAndMortyApp
   cd RickAndMortyApp
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Ejecuta la aplicación:
   ```bash
   ng serve
   ```

4. Abre el navegador en:
   ```text
   http://localhost:4200
   ```

---

## **Arquitectura**

Este proyecto sigue la arquitectura **Backend for Frontend (BFF)**:

- **Frontend**:
  - Consume exclusivamente el BFF.
  - Desarrollado en Angular 19 utilizando standalone components.
  - Implementa paginación y filtros.

- **Backend (BFF)**:
  - Implementado en .NET 8.
  - Proporciona un punto de acceso unificado para el frontend.
  - Llama a la API pública de Rick and Morty para obtener los datos necesarios.

- **API Externa**:
  - [Rick and Morty API](https://rickandmortyapi.com).

---

## **Links a Repositorios**

1. **Backend (RickAndMortyAPI)**: [Ver repositorio](https://github.com/Giovasdf/RickAndMortyAPI)
2. **Frontend (RickAndMortyApp)**: [Ver repositorio](https://github.com/Giovasdf/RickAndMortyApp)

---

## **Cómo Contribuir**

1. Haz un fork del proyecto.
2. Crea una nueva rama:
   ```bash
   git checkout -b feature/nueva-funcion
   ```

3. Realiza los cambios y commitea:
   ```bash
   git commit -m "Agrega nueva función"
   ```

4. Haz un push a tu rama:
   ```bash
   git push origin feature/nueva-funcion
   ```

5. Abre un pull request.

---

## **Licencia**

Este proyecto está bajo la licencia [MIT](LICENSE).

---

## **Contacto**

Si tienes preguntas o comentarios, puedes contactarme a través de:
- **Email Español**: [hola@gmolina.tech](mailto:hola@gmolina.tech)
- **Email English**: [hello@gmolina.tech](mailto:hello@gmolina.tech)

- **LinkedIn**: [Giovanni Molina](https://www.linkedin.com/in/giovannimg/)
