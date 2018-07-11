//Objective-c

void uncaughtExceptionHandler(NSException *exception)
{
   //アプリクラッシュ時のログ出力
    NSLog(@"%@", exception);
}


- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
    NSSetUncaughtExceptionHandler(&uncaughtExceptionHandler);
    return YES;
}
 
