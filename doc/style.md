  ## 样式说明
  
  1. Material-UI 提供了一个 CssBaseline 组件, 用于启动一个优雅、一致且简单的基线。
  1. CSS 注入顺序：...内联 > styled-jsx > jss > styled-components >。 选择一种使用。
  1. 定制方案：mui 提供的 classes 属性、jss、styled-components、内联样式, Theme nesting
  1. body > page > section > container > component

  ```
    // 使用Material-UI默认的CSS-in-js方案，通过 jss 的 withStyles() 定制
    <Button className={classNames(classes.root, className)} {...other}>
      {children || 'class names'}
    </Button>
    // 通过 mui提供的 classess属性深度定制
    <Button
      classes={{
        root: classes.root, // class name, e.g. `classes-nesting-root-x`
        label: classes.label, // class name, e.g. `classes-nesting-label-x`}}>
      classes nesting
    </Button>

    // 通过内联样式
    <Button style={style}>inline-style</Button>;

    // 动态样式
    <Button  className={classNames(classes.button, {
      [classes.buttonBlue]: this.state.color === 'blue',})}>
    {'Class name branch'}</Button>

    // 根据 theme 设置
    <Button color="primary">Primary</Button>
    <Button color="secondary">Secondary</Button>

    // nextjs 提供的 CSS-in-js 方案 styled-jsx
    <style jsx>
    {`
      $color: blue;

      .hello {
        background-color: ${backgroundColor};
        padding: 100px;
        text-align: center;
        transition: 100ms ease-in background;
        &:hover {
          color: $color;
        }

        @media only screen and (max-width: 480px) {
          font-size: 20px;
        }
      }
      `}
    </style>

    // 其他CSS-in-js方案：styled-components
    const Button = styled.button`
      background: transparent;
      border-radius: 3px;
      border: 2px solid palevioletred;
      color: palevioletred;
      margin: 0.5em 1em;
      padding: 0.25em 1em;

      ${props => props.primary && css`
        background: palevioletred;
        color: white;
      `}
    `;

    const Container = styled.div`
      text-align: center;`
  ```