Recently, we've been working on a project and have encountered the following issue when running an API:

[17:43:28 ERR] Method not found: 'Void Volo.Abp.DynamicProxy.IAbpInterceptor.Intercept(Volo.Abp.DynamicProxy.IAbpMethodInvocation)'.
System.MissingMethodException: Method not found: 'Void Volo.Abp.DynamicProxy.IAbpInterceptor.Intercept(Volo.Abp.DynamicProxy.IAbpMethodInvocation)'.
   at Volo.Abp.Castle.DynamicProxy.CastleAbpInterceptorAdapter`1.InterceptSyncMethod(IInvocation invocation, IInvocationProceedInfo proceedInfo)
   at Volo.Abp.Castle.DynamicProxy.CastleAbpInterceptorAdapter`1.Intercept(IInvocation invocation)
   at Castle.DynamicProxy.AbstractInvocation.Proceed()
   at Castle.Proxies.IBasicRepository`1Proxy_2.GetWaitingList(Int32 maxResultCount)
   at Volo.Abp.BackgroundJobs.BackgroundJobStore.GetWaitingJobs(Int32 maxResultCount)
   at Volo.Abp.BackgroundJobs.BackgroundJobWorker.DoWork()
   at Volo.Abp.BackgroundWorkers.PeriodicBackgroundWorkerBase.Timer_Elapsed(Object sender, EventArgs e)

   What could be possibly made to work it out?
