# webgl
learn webgl

拿到所有的顶点之后先执行顶点着色器进行图形装配，然后光栅化得到所有片元，最后才一个一个的执行片元着色器，
光栅化过程中会对片元着色器中的变量vary进行插值，所以顶点着色器中的vary和片元着色器中的vary实际上不是同一个东西

顶点数据：vertex。
索引数据：index。描述顶点绘制顺序  drawElements
法向量数据：normal。描述顶点法向量，用于计算光照，从 入射光颜色 * 表面基底色 * cos0，入射角是如何光和法向量的夹角

光：平行光，环境光，点光源