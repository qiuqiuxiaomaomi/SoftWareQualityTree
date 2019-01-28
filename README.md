# SoftWareQualityTree
软件质量技术研究


<pre>
代码质量锁涉及的5个方面

      1：编码标准：命名规范，代码风格等
      2：代码重复：重复代码需要提炼成公共方法或者组件化
      3：代码覆盖率：测试代码能够运行到的代码比率，这关系到代码的功能性和稳定性。
      5：依赖项分析：代码的依赖关系怎么样？耦合关系怎么样？是否有循环依赖？是否符合高内聚
                   低耦合的原则？
      6：复杂度分析：

      上面解释了代码质量相关的5个方面，在实际开发环境中，已经有很多工具为我们解决以上5个方
      面的问题，下列5个eclipse插件分别对这5个问题有很好的支持：

          1） 编码标准：CheckStyle  插件URL：http://eclipse-cs.sourceforge.net/update/

          2）代码重复：PMD的CPD  插件URL：http://pmd.sourceforge.net/eclipse/

          3）代码覆盖率：Eclemma 插件URL：http://update.eclemma.org

          5）依赖项分析：JDepend 插件URL：http://andrei.gmxhome.de/eclipse/

          6）复杂度分析：Eclipse Metric  插件URL：http://metrics.sourceforge.net/update
</pre>

<pre>
Solar与idea结合

      java项目利用sonar平台进行代码指标度量。比如复杂度、重复度、单测覆盖和数量、坏味道、bugs；

      sonar jar包使用过程中，涉及到几个插件
 
          Pmd 它是一个基于静态规则集的Java源码分析器，它可以识别出潜在的如下问题：
              – 可能的bug——空的try/catch/finally/switch块。
              – 无用代码(Dead code)：无用的本地变量，方法参数和私有方法。
              – 空的if/while语句。
              – 过度复杂的表达式——不必要的if语句，本来可以用while循环但是却用了for循环。
              – 可优化的代码：浪费性能的String/StringBuffer的使用。

          FindBugs 它用来查找Java代码中存在的bug。它使用静态分析方法标识出Java程序中上百种潜在的不同类型的错误。

          Checkstyle 它定义了一系列可用的模块，每一个模块提供了严格程度(强制的，可选的…)可配置的检查规则。规则可以触发通
                     知(notification)，警告(warning)和错误(error)。
</pre>