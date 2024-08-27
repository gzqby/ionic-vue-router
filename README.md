# ionic-vue-router

This project is derived from @ionic/vue-router

If you are using ionic to develop applications and need to deploy them to a web environment, you may need it

https://github.com/ionic-team/ionic-framework/issues/29721
## usage
```
// import { createRouter, createWebHistory } from "@ionic/vue-router";
import { createRouter, createWebHistory } from "ionic-vue-router";
import { RouteRecordRaw } from "vue-router";

const routes: Array<RouteRecordRaw> = [
  {
    path: "/",
    component: () => import("@/views/index.vue"),
  },
];

const router = createRouter({
  history: createWebHistory(import.meta.env.BASE_URL),
  routes,
});

export default router;

```