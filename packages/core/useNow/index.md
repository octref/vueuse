---
category: Animation
---

# useNow

Reactive current Date instance.

## Usage

```js
import { useNow } from '@vueuse/core'

const now = useNow()
```

```js
const { now, pause, resume } = useNow({ controls: true })
```


<!--FOOTER_STARTS-->
## Type Declarations

```typescript
export interface UseNowOptions<Controls extends boolean> {
  /**
   * Expose more controls
   *
   * @default false
   */
  controls?: Controls
  /**
   * Update interval, or use requestAnimationFrame
   *
   * @default requestAnimationFrame
   */
  interval?: "requestAnimationFrame" | number
}
/**
 * Reactive current Date instance.
 *
 * @see   {@link https://vueuse.org/useNow}
 * @param options
 */
export declare function useNow(options?: UseNowOptions<false>): Ref<Date>
export declare function useNow(
  options: UseNowOptions<true>
): {
  now: Ref<Date>
} & Pausable
```

## Source

[Source](https://github.com/vueuse/vueuse/blob/main/packages/core/useNow/index.ts) • [Demo](https://github.com/vueuse/vueuse/blob/main/packages/core/useNow/demo.vue) • [Docs](https://github.com/vueuse/vueuse/blob/main/packages/core/useNow/index.md)


<!--FOOTER_ENDS-->