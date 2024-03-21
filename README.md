#### loading.ts

- 位置 src/plugins/loading.ts
- logo systemLogo logo.svg
- 主题色 themeColor src/theme/setting.ts
- 加载文字 langs 对应 system.title

#### 登录页面

- 位置 src/view/_builtin/login

- logo <SystemLogo />组件

  本地svg用法 src/assets/svg-icon
  新增 xxx.svg
  用法 <icon-local-xxx />

#### 接口配置

- npm run dev => "dev": "vite --mode test",
- 修改 .env.test VITE_SERVICE_BASE_URL
- 修改 utils/service.ts createProxyPattern() 修改 server 请求前缀

#### 点击登录

- 位置 /src/views/builtin/login/modules/pwd-login.vue
- handleSubmit()  => useAuthStore login
- 修改登录 .vue  authStore fetchLogin ts等对应登录相关字段
- 到此可以成功调取新的登录接口
- 系统 message error 'the backend request error'
