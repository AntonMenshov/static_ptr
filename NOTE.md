[Original paper](https://habr.com/ru/articles/665632/)

[`aligned_storage`](https://en.cppreference.com/w/cpp/types/aligned_storage) is 
[deprecated](https://stackoverflow.com/questions/71828288/why-is-stdaligned-storage-to-be-deprecated-in-c23-and-what-to-use-instead), 
so the following construct is probably more useful:

`alignas(align) std::byte buf_[buffer_size];`
