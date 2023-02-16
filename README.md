# React-router | JSON Server | D2

---

## install react router latest

**_npm install react-router-dom@latest_**

---

## install JSON Server globally

**_npm install -g json-server_**

- start json server on port 4000

**_json-server -p 4000 -w ./data/db.json_**

---

## old way

![react router old way](./src/assets/img/router-old-way.png)

- now we can use server rendering if we use browser url

![navigate with browser url](./src/assets/img/navigate-browser-url.png)

- but when we use Link or NavLink we use SPA rendering on client side

![navigate on client side](./src/assets/img/client-side-rendering.png)

- this is the same

![navigate on client side](./src/assets/img/path-to-root.png)

- when we use Navlink we get class active - always use NavLink

---

## new way

- instead of Browser router and Routes we will use function createBrowserRouter

<https://reactrouter.com/en/main/routers/picking-a-router>

- in src folder we will have folder for pages and layouts

![src folder](./src/assets/img/folder-src.png)

- import createBrowserRouter
- import createRoutesFromElement
- import RouteProvider
- inside createBrowserRouter we don't use Routes - we use Route
- inside parent route we have path=" / " element={RouteLayout}

![ap.jsx file](./src/assets/img/app.jsx-file.png)

- RouteLayout component

![routeLayout component](./src/assets/img/route-layout.png)

---

### Nested routes

- nested routes

![routeLayout component](./src/assets/img/nested-routes.png)

- help layout component

![helpLayout component](./src/assets/img/help-layout.png)

- src folder

![src folder](./src/assets/img/src-folder2.png)

- page not found

![page not found](./src/assets/img/page-not-found.png)

---

## Loaders

- we use loaders to load data before component renders

- we don't need to use **useEffect**

- make Loader function

![loader function](./src/assets/img/loaderFunction.png)

- in route use that function

![loader function in route](./src/assets/img/loader-in-route.png)

- in component use useLoaderData()

![useLoaderData](./src/assets/img/useLoaderData.png)
