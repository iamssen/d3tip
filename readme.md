# D3 Tooltip

## Sample
[Web Site](http://iamssen.github.io/d3tip/) ← [Source Code](https://github.com/iamssen/d3tip/tree/gh-pages)

## Install
```sh
npm install d3tip --save
npm install d3-selection --save
npm install types.d3 --save # d3 4.x typings
```

```typescript
import {select} from 'd3-selection';
import d3tip from 'd3tip';
import 'd3tip/index.css'; // Default tooltip style. If you don't need default style. you have not to import this.

d3.select('#button')
  .datum('HELLO WORLD')
  .call(d3tip({
    html: d => d.toString()
  }))
```

## Options
- `html: string|(d?:any, i?:number, nodes?:Node[]) => string`
- `classed?: string[]|(d?:any, i?:number, nodes?:Node[]) => string[]`
- `distance?: number`
- `target?: string = 'pointer' | 'element'`
- `position?: string|(d?:any, i?:number, nodes?:Node[]) => string = 'left' | 'right' | 'top' | 'bottom' | 'topLeft' | 'topRight' | 'bottomLeft' | 'bottomRight'`

----------

# Archive

- [ ] 나중에 Graphics 작업을 할때 분명 다시 필요해질 가능성이 있음. React 등과 결합해서 다시 만들 필요가 있음. 기반하고 있는 작동 Code들은 정리해서 옮길 필요가 있음.
