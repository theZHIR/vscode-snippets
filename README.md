# React-TypeScript Snippets

Simple collection of React-TypeScript Snippets.

## Snippets

### Import

| Trigger  | Content |
| -------: | ------- |
| `imr→`   | import React |
| `imrd→`  | import ReactDOM |

### React

| Trigger  | Content |
| -------: | ------- |
| `cc→`    | class component |
| `ccp→`   | class component with `Props` |
| `ccs→`   | class component with `State` |
| `ccc→`   | `constructor() {…}` |
| `sfc→`   | stateless function component |
| `sfcp→`  | stateless function component with `Props` |
| `cwm→`   | `componentWillMount() {…}` |
| `cdm→`   | `componentDidMount() {…}` |
| `cwr→`   | `componentWillReceiveProps() {…}` |
| `scu→`   | `shouldComponentUpdate() {…}` |
| `cwu→`   | `componentWillUpdate() {…}` |
| `cdu→`   | `componentDidUpdate() {…}` |
| `cwun→`  | `componentWillUnmount() {…}` |
| `ss→`    | `this.setState({…})` |
| `ssf→`   | `this.setState(() => {…})` |
| `dp→`    | `defaultProps = {…}` |
| `refs→`  | `refs: {…}` |

## Full Expansions

### Import

#### imr - import React
```
import * as React from 'react';
```

#### imrd - import ReactDOM
```
import [* as ReactDOM] from 'react-dom';
```

### React

#### cc - class component
```
export class [FileName] extends React.Component<{}, {}> {
  render() {
    return …
  }
}
```

#### ccp - class component with `Props`
```
interface Props {}

export class [FileName] extends React.Component<Props, {}> {
  render() {
    return …
  }
}
```

#### ccs - class component with `State`
```
interface Props {}

interface State {}

export class [FileName] extends React.Component<Props, State> {
  constructor(props: Props) {
    super(props);
    this.state = {};
  }

  render() {
    return …
  }
}
```

#### ccc - constructor() {…}
```
constructor(props: Props) {
  super(props);
  …
}
```

#### sfc - stateless function component
```
export const [FileName]: React.SFC<{}> = () => {
  return …
};
```

#### sfcp - stateless function component with `Props`
```
interface Props {}

export const [FileName]: React.SFC<Props> = props => {
  return …
};
```

#### cwm - componentWillMount() {…}
```
componentWillMount(): void {
  …
}
```

#### cdm - componentDidMount() {…}
```
componentDidMount(): void {
  …
}
```

#### cwr - componentWillReceiveProps() {…}
```
componentWillReceiveProps(nextProps: Props): void {
  …
}
```

#### scu - shouldComponentUpdate() {…}
```
shouldComponentUpdate(nextProps: Props, nextState: State): boolean {
  …
}
```

#### cwu - componentWillUpdate() {…}
```
componentWillUpdate(nextProps: Props, nextState: State): void {
  …
}
```

#### cdu - componentDidUpdate() {…}
```
componentDidUpdate(prevProps: Props, prevState: State): void {
  …
}
```

#### cwun - componentWillUnmount() {…}
```
componentWillUnmount(): void {
  …
}
```

#### ss - setState({…})
```
this.setState({ … });
```

#### ssf - setState(() => {…})
```
this.setState((prevState: State, props: Props) => {
  …
});
```

#### dp - defaultProps = {…}
```
[const|static] defaultProps: Partial<Props> = {
  …
};
```

#### refs - refs: {…}
```
refs: {
  [key: string]: Element;
  …
};
```
