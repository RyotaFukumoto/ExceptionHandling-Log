//Objective-c

- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
    NSSetUncaughtExceptionHandler(&uncaughtExceptionHandler);
    return YES;
}
 
void uncaughtExceptionHandler(NSException *exception)
{
   
    NSLog(@"%@", exception);
}
