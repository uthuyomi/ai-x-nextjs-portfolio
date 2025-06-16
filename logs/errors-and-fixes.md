# 🧯 Error Log & Fix History

---

## ❌ Error 1: Type Mismatch

**Message**  
```
Type 'Posts[]' is not assignable to type 'Post[]'
```

**Cause**  
- `ArchiveItem` component was incorrectly using `Posts` (undefined or incorrect type)
- The correct type is `Post`, defined in `types.ts`

**Fix**  
```ts
type Props = { posts: Post[]; noimg: string };
```
- Ensure `Post` is properly imported from `@/types/types`

---

## ❌ Error 2: Undefined image URL

**Message**  
```
Cannot read properties of undefined (reading 'source_url')
```

**Cause**  
- Some posts do not have a featured image, so `_embedded["wp:featuredmedia"]` is `undefined`

**Fix**  
- Used optional chaining (`?.`) to avoid runtime error
- Fallback image (`noimg`) provided in case thumbnail is missing

```ts
const thumbnail = post._embedded?.["wp:featuredmedia"]?.[0]?.source_url;
```

---
