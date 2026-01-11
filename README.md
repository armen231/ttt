# Дальнейшеее обучение
после обучения изучить материал на странице https://react.dev/learn/creating-a-react-app,
                                               https://react.dev/learn/build-a-react-app-from-scratch,
                                               https://react.dev/learn/editor-setup,
                                               https://react.dev/learn/typescript,
                                               https://react.dev/learn/react-compiler (весь раздел)
                                               (посмотреть первые 4 материала в главе "Начало работы" ),
						https://legacy.reactjs.org/docs/optimizing-performance.html,
						https://github.com/immerjs/use-immer,
                        https://github.com/immerjs/use-immer#useimmerreducer,
                        https://react.dev/reference/react/useImperativeHandle,
***
# Неизученные материалы
1. https://react.dev/reference/react-compiler/gating
2. https://react.dev/reference/react-compiler/logger
***                        
# Подсказки:
1. преобразование html в формат jsx => https://transform.tools/html-to-jsx
2. Инструменты разработчика React для chrom => https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en
                                  для edge => https://microsoftedge.microsoft.com/addons/detail/react-developer-tools/gpphkfbcpidddadnkolkpfckpihlkkil
***                                  
# Описание изменений:
1. compilationMode: Параметр compilationMode определяет, как React Compiler выбирает функции для компиляции. https://react.dev/reference/react-compiler/compilationMode
2. compilationMode: применение параметра => babel.config.js
***
# Предупреждение
## compilationMode
1. Режим 'infer' требует, чтобы функции соответствовали соглашениям об именовании React
2. Использование режима 'all' может негативно сказаться на производительности из-за компиляции служебных функций
3. Режим 'syntax' требует Flow и не будет работать с TypeScript
4. Независимо от режима, функции с директивой "use no memo" всегда пропускаются
## panicThreshold
1. В производственных сборках всегда следует использовать 'none'
2. Сбои при сборке не позволяют собрать приложение
3. Компилятор автоматически обнаруживает и пропускает проблемный код с 'none'
4. Более высокие пороговые значения полезны только во время разработки для отладки
