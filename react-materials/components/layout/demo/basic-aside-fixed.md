---
title: Aside 吸顶
order: 2
iframe: true
width: 960
importStyle: true
---

Aside Header Footer 固定位置布局。

````jsx
import React, { Component } from 'react';
import ReactDOM from 'react-dom';
import Layout from '@icedesign/layout';

class App extends Component {
  render() {
    return (
      <Layout fixable={true}>
        <Layout.Aside>
          <br />
          Aside
        </Layout.Aside>
        <Layout.Section scrollable={true}>
          <Layout.Header>&nbsp;&nbsp;&nbsp;&nbsp;Header</Layout.Header>
          <Layout.Main>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
            <p style={{ height: 200 }}>内容可滚动</p>
          </Layout.Main>
          <Layout.Footer>Footer</Layout.Footer>
        </Layout.Section>
      </Layout>
    );
  }
}

ReactDOM.render(<App />, mountNode);
````

````css
.ice-layout {
  color: #fff;
  text-align: center;
  background-color: #eee;
}
.ice-layout-header {
  line-height: 50px;
  background-color: #84B0E7 !important;;
}
.ice-layout-aside {
  background-color: rgba(27, 115, 225, 0.7) !important;;
}
.ice-layout-main {
  line-height: 120px;
  background-color: rgba(27, 115, 225, 1);
}
.ice-layout-footer {
  line-height: 50px;
  background-color: #84B0E7;
}
````
