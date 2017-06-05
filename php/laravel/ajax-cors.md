# laravel ajax 跨域问题


#### 定义一个中间件


```
public function handle($request, Closure $next)
   {
       /*$response = $next($request);
       $response->header('Access-Control-Allow-Origin', '*');
       $response->header('Access-Control-Allow-Headers', 'X-Requested-With,X_Requested_With');*/

       $response = $next($request);
       $response->header('Access-Control-Allow-Origin', '*');
       $response->header('Access-Control-Allow-Headers', 'Origin, Content-Type, Cookie, Accept, Authorization');
       $response->header('Access-Control-Allow-Methods', 'GET, POST, PATCH, PUT, OPTIONS');
       $response->header('Access-Control-Allow-Credentials', 'true');

       return $response;
   }

```


#### [barryvdh/laravel-cors 插件](https://github.com/barryvdh/laravel-cors)
