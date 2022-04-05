# Somos más ONG
## El proyecto consta en desarrollar el Frontend de una página web para Somos más.
- Biblioteca: REACT JS
- Metodología: SCRUM utilizando Jira Software.
- Control de versiones: GIT - GITHUB
- Herramientas principales: REDUX/TOOLKIT -  ESLINT - CHAKRA UI  - AXIOS - REACT ROUTER DOM - FORMIK  - React Testing Library

### Home
![ScreenShot](/public/images/image_0.png)

### Error Login
![ScreenShot](/public/images/image_1.png)
### Campaign Toys
![ScreenShot](/public/images/image_2.png)

### Dahsboard Admin
![ScreenShot](/public/images/image_3.png)

### Backoffice
![ScreenShot](/public/images/image_4.png)


## Ong Client

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app), using the [Redux](https://redux.js.org/) and [Redux Toolkit](https://redux-toolkit.js.org/) template.

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### Como utilizar el Setup Progress linear
Implementacion del componente progreso linear
El spinner fue hecho para el estado de carga de la pantalla.

**value**: recibe un valor de 0 a 100. El 0 es el estado inicial y el 100 es el estado final que indica que ya esta cargado.

# `Loaders`


AlertServicie
The path is accessed via the (http://localhost:3000/alert) path.
A service was created in this file where three alert functions are exported (confirmation, error, information). They receive props, in case they are null they have default values.

Loader component uses two Loaders from the Chakra-UI Library, these are following links:

- Spinner: https://chakra-ui.com/docs/components/feedback/spinner
- Progress: https://chakra-ui.com/docs/components/feedback/progress

Loader component returns one of two types of loaders:

- Progress Bar (default).
- Spinner (passing the type='spinner' prop)

## `Loaders Use`

Loader must be rendered whenever an HTTP request isnt fulfilled. (Conditional Rendering).

### `Loaders props`

Loader component receives the following props:

**type** : String. can be 'spinner' to display an spinner, or null to display a progress bar (default option).

**size** : Must be one of the followings: ( 'xs','sm','md','lg')

### Como implementar Skeleton

Skeleton se utiliza para mostrar un feedback al usuario cuando se esté realizando la carga de contenido.

Para incorporarlo se debe importar el componente reutilizable <SkeletonGroup />. Y se puede hacer uso de las siguientes propiedades, entre otras. Ejemplo:

<SkeletonGroup skeletonItems={["block", "text", "circle", "circle"]} />
