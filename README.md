Run "npm install" and "./node_modules/.bin/nyc node index.js". Get back:

        /Users/philip/src/nyc-bug/index.js:2
        cov_235y2cz5ul=function(){return actualCoverage;};}return actualCoverage;}cov_235y2cz5ul();function f(){cov_235y2cz5ul().f[0]++;cov_235y2cz5ul().s[0]++;return0n;}cov_235y2cz5ul().s[1]++;f();
                                                                                                                                                                ^

        ReferenceError: return0n is not defined
            at f (/Users/philip/src/nyc-bug/index.js:2:153)
            at Object.<anonymous> (/Users/philip/src/nyc-bug/index.js:2:187)
            at Module._compile (internal/modules/cjs/loader.js:955:30)
            at Module.replacementCompile (/Users/philip/src/nyc-bug/node_modules/append-transform/index.js:60:13)
            at Module._extensions..js (internal/modules/cjs/loader.js:991:10)
            at Object.<anonymous> (/Users/philip/src/nyc-bug/node_modules/append-transform/index.js:64:4)
            at Module.load (internal/modules/cjs/loader.js:811:32)
            at Function.Module._load (internal/modules/cjs/loader.js:723:14)
            at Function.Module.runMain (internal/modules/cjs/loader.js:1043:10)
            at internal/main/run_main_module.js:17:11
        ----------|---------|----------|---------|---------|-------------------
        File      | % Stmts | % Branch | % Funcs | % Lines | Uncovered Line #s 
        ----------|---------|----------|---------|---------|-------------------
        All files |     100 |      100 |     100 |     100 |                   
         index.js |     100 |      100 |     100 |     100 |                   
        ----------|---------|----------|---------|---------|-------------------

