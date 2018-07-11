//Objective-c

void uncaughtExceptionHandler(NSException *exception)
{
    NSLog(@"%@", exception);
//アプリクラッシュ時のログ出力
}


- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
    NSSetUncaughtExceptionHandler(&uncaughtExceptionHandler);
    return YES;
}
 
