# firstproject
promise asyinc await
var sleep = function(time){
    return new Promise(function(resolve,reject){
        setTimeout(function(){
            console.log("中间");
            resolve();
        },time);
    });
}
var start = async function(){
    console.log("start loading..");
    // sleep().then(function(){
    //     console.log("中间");
    // });
    await sleep(3000);
    console.log("end loading...");
}
start();

