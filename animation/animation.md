## 动画组成
- animation: 描述动画的各个规则
- @keyframe: 指定动画开始、结束以及中间点样式的关键帧

## animation
用于配置动画时间、时长以及其他动画细节
### 子属性
- animation-name: 指定由 `@keyframe` 描述的关键帧名称；
- animation-duration: 设置动画一个周期的时长；
- animation-delay: 设置延时，及从元素加载完成之后到动画序列开始执行的这段时间，可以设置负值，使动画提前进行；
- animation-direction: 设置动画在每次运行完后是反向运行还是重新回到开始位置重复运行；
- animation-iteration-count: 设置动画重复次数，可以指定 `infinite` 无限次重复动画；
- animation-play-state: 允许暂停和恢复动画；
- animation-timing-function: 设置动画速度，即通过建立加速度曲线，设置动画在关键帧之间如何变化；
  - cubic-bezier-timing-function: 三次内赛尔曲线缓动函数
    - ease: 低速开始，然后加快，在结束前变慢
    - ease-in: 低速开始
    - ease-out: 低速结束
    - ease-in-out: 以低速开始和结束
    - linear: 匀速
    - cubic-bezier(): 自定义三次内赛尔曲线
  - step-timing-function 
    - step-start
    - step-end
    - steps(): 
- animation-fill-mode: 执行动画执行前后如何为目标元素应用样式；
  - animation-fill-mode: backwards: 可以让元素在动画开始之前的样式为动画运行时的第一帧，动画结束后的样式则恢复为 css 规则设定的样式
  - animation-fill-mode: forwards: 元素在动画开始之前的样式为css对着设定的样式，而动画结束后的样式则由执行期间遇到的最后一个关键帧计算值（即停留在最后一帧）
  - animation-fill-mode: both: 兼顾以上两种模式的特点，可以使得动画开始的样式为动画运行时的第一帧，动画结束后停留在最后一帧
- @keyframe 规则: 动画实际表现。