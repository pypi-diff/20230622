# Comparing `tmp/fbgemm_gpu_nightly_cpu-2023.6.21-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2023.6.22-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,40 +1,40 @@
-Zip file size: 3196095 bytes, number of entries: 38
--rw-r--r--  2.0 unx      567 b- defN 23-Jun-21 13:01 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx    14920 b- defN 23-Jun-21 13:01 fbgemm_gpu/_fbgemm_gpu_docs.py
--rw-r--r--  2.0 unx     2747 b- defN 23-Jun-21 13:01 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jun-21 13:01 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10709064 b- defN 23-Jun-21 13:01 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5648 b- defN 23-Jun-21 13:01 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2339 b- defN 23-Jun-21 13:01 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2477 b- defN 23-Jun-21 13:01 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7682 b- defN 23-Jun-21 13:01 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4005 b- defN 23-Jun-21 13:01 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     5745 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     6661 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx    19751 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2170 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3433 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    61087 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    80494 b- defN 23-Jun-21 13:01 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    39550 b- defN 23-Jun-21 13:01 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      910 b- defN 23-Jun-21 13:01 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx     1603 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4717 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     3354 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3112 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     1906 b- defN 23-Jun-21 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3354 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3062 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     2617 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     3370 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3370 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     5005 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     7014 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3105 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
--rw-r--r--  2.0 unx     4961 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
--rw-r--r--  2.0 unx     4250 b- defN 23-Jun-21 12:59 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     2934 b- defN 23-Jun-21 13:01 fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-21 13:01 fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-21 13:01 fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4171 b- defN 23-Jun-21 13:01 fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/RECORD
-38 files, 11032089 bytes uncompressed, 3189073 bytes compressed:  71.1%
+Zip file size: 3196090 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      567 b- defN 23-Jun-22 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx    14920 b- defN 23-Jun-22 12:59 fbgemm_gpu/_fbgemm_gpu_docs.py
+-rw-r--r--  2.0 unx     2747 b- defN 23-Jun-22 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jun-22 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10709064 b- defN 23-Jun-22 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5648 b- defN 23-Jun-22 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Jun-22 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2477 b- defN 23-Jun-22 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7682 b- defN 23-Jun-22 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4005 b- defN 23-Jun-22 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     5745 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     6661 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx    19751 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3433 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    61087 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    80494 b- defN 23-Jun-22 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    39550 b- defN 23-Jun-22 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      910 b- defN 23-Jun-22 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4717 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3112 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_approx_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     1906 b- defN 23-Jun-22 12:53 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     2617 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     3370 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3370 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     5005 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     7014 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3105 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py
+-rw-r--r--  2.0 unx     4961 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
+-rw-r--r--  2.0 unx     4250 b- defN 23-Jun-22 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     2934 b- defN 23-Jun-22 12:59 fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-22 12:59 fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-22 12:59 fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4171 b- defN 23-Jun-22 12:59 fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/RECORD
+38 files, 11032089 bytes uncompressed, 3189068 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -96,20 +96,20 @@
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -157013,15 +157013,15 @@
 	lea    0x380(%rsp),%r13
 	call   147610 <__cxa_atexit@plt>
 	mov    %r13,%rdx
 	lea    0x77a8ac(%rip),%rsi        
 	mov    %r12,%rdi
 	call   146980 <std::basic_string<char, std::char_traits<char>, std::allocator<char> >::basic_string<std::allocator<char> >(char const*, std::allocator<char> const&)@plt>
 	mov    $0x363,%r9d
-	mov    $0x7c0001,%ecx
+	mov    $0x7d0001,%ecx
 	mov    %r12,%rdx
 	lea    0x782abb(%rip),%r8        # 974c20 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1a80>
 	mov    $0x1,%esi
 	lea    0x84d64f(%rip),%rdi        # a3f7c0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x200>
 	call   147ec0 <torch::Library::Library(torch::Library::Kind, std::string, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x3d0(%rsp),%rax
 	mov    0x83fbbb(%rip),%rbx        
@@ -157683,15 +157683,15 @@
 	lea    0x2e0(%rsp),%r13
 	call   147610 <__cxa_atexit@plt>
 	mov    %r13,%rdx
 	lea    0x77995c(%rip),%rsi        
 	mov    %r12,%rdi
 	call   146980 <std::basic_string<char, std::char_traits<char>, std::allocator<char> >::basic_string<std::allocator<char> >(char const*, std::allocator<char> const&)@plt>
 	mov    $0xc0,%r9d
-	mov    $0x370001,%ecx
+	mov    $0x380001,%ecx
 	mov    %r12,%rdx
 	lea    0x7840bb(%rip),%r8        # 977170 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x350>
 	mov    $0x1,%esi
 	lea    0x84cbff(%rip),%rdi        
 	call   147ec0 <torch::Library::Library(torch::Library::Kind, std::string, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x330(%rsp),%rax
 	mov    0x83ec6b(%rip),%rbx        
@@ -158438,15 +158438,15 @@
 	lea    0x84bbe2(%rip),%rsi        # a3fdc0 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x80>
 	mov    %rbp,%rdi
 	call   147610 <__cxa_atexit@plt>
 	mov    $0x1,%esi
 	lea    0x3b130e(%rip),%rdx        
 	lea    0x84bb67(%rip),%rdi        # a3fd60 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x20>
 	lea    0x786818(%rip),%r9        # 97aa18 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x2738>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x7787e7(%rip),%rcx        
 	movl   $0x695,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	pop    %rax
 	mov    %rbp,%rdi
 	pop    %rdx
 	lea    0x84bb3b(%rip),%rsi        # a3fd60 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x20>
@@ -158522,15 +158522,15 @@
 	lea    0x84bb65(%rip),%rsi        # a3fee0 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x1a0>
 	mov    %rbp,%rdi
 	call   147610 <__cxa_atexit@plt>
 	mov    $0x1,%esi
 	lea    0x5f2011(%rip),%rdx        # 7e63a0 <fbgemm_gpu::recat_embedding_grad_output_mixed_D_cpu(at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x2d60>
 	lea    0x84baea(%rip),%rdi        # a3fe80 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x140>
 	lea    0x78902b(%rip),%r9        # 97d3c8 <typeinfo name for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, long)@@Base+0x108>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x77864a(%rip),%rcx        
 	movl   $0x51,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	pop    %rax
 	mov    %rbp,%rdi
 	pop    %rdx
 	lea    0x84babe(%rip),%rsi        # a3fe80 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x140>
@@ -158559,15 +158559,15 @@
 	lea    0x84bb62(%rip),%rsi        # a3ffa0 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x260>
 	mov    %rbp,%rdi
 	call   147610 <__cxa_atexit@plt>
 	mov    $0x1,%esi
 	lea    0x5f653e(%rip),%rdx        
 	lea    0x84bae7(%rip),%rdi        # a3ff40 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x200>
 	lea    0x789538(%rip),%r9        # 97d998 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x298>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x778587(%rip),%rcx        
 	movl   $0x1c0,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	pop    %rax
 	mov    %rbp,%rdi
 	pop    %rdx
 	lea    0x84babb(%rip),%rsi        # a3ff40 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x200>
@@ -158597,15 +158597,15 @@
 	lea    0x84bb52(%rip),%rsi        # a40060 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x320>
 	mov    %rbp,%rdi
 	call   147610 <__cxa_atexit@plt>
 	mov    $0x1,%esi
 	lea    0x67914e(%rip),%rdx        
 	lea    0x84bad7(%rip),%rdi        # a40000 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x2c0>
 	lea    0x78bd58(%rip),%r9        # 980288 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0xc68>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x7784b7(%rip),%rcx        
 	movl   $0xa1c,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	pop    %rax
 	mov    %rbp,%rdi
 	pop    %rdx
 	lea    0x84baab(%rip),%rsi        # a40000 <c10::detail::getMaybeFakeTypePtr_<c10::ArrayRef<c10::SymInt>, false>::call()::type@@Base+0x2c0>
@@ -158637,15 +158637,15 @@
 	mov    %cx,0x4(%rdx)
 	cmp    %rbx,%rax
 	jne    1f470e <std::__throw_bad_weak_ptr()@@Base+0xa3ec2>
 	lea    0x10(%rsp),%rbp
 	mov    %rdx,0x10(%rsp)
 	mov    $0x26,%r9d
 	lea    0x790b12(%rip),%r8        # 985100 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PackSegmentsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x320>
-	mov    $0x370001,%ecx
+	mov    $0x380001,%ecx
 	mov    %rbp,%rdx
 	mov    $0x1,%esi
 	lea    0x84bbfe(%rip),%rdi        # a40200 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x18>
 	call   147ec0 <torch::Library::Library(torch::Library::Kind, std::string, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x10(%rsp),%rax
 	lea    -0x18(%rax),%rdi
 	cmp    %rbx,%rdi
@@ -158735,15 +158735,15 @@
 	lea    0x84bbcc(%rip),%rdi        # a40380 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x198>
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	mov    0x83efd0(%rip),%rbp        
 	lea    0x841839(%rip),%rdx        # a36000 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0x8508>
 	lea    0x84bbb2(%rip),%rsi        # a40380 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x198>
 	mov    %rbp,%rdi
 	call   147610 <__cxa_atexit@plt>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x790b5d(%rip),%r9        # 985340 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PackSegmentsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x560>
 	lea    0x77820a(%rip),%rcx        
 	lea    0x6a577f(%rip),%rdx        
 	mov    $0x1,%esi
 	lea    0x84bb23(%rip),%rdi        # a40320 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x138>
 	movl   $0xac,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
@@ -158763,15 +158763,15 @@
 	lea    0x8417a7(%rip),%rdx        # a36000 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0x8508>
 	lea    0x84ba60(%rip),%rsi        # a402c0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0xd8>
 	call   147610 <__cxa_atexit@plt>
 	mov    $0x1,%esi
 	lea    0x6a5a2f(%rip),%rdx        
 	lea    0x84b9e8(%rip),%rdi        # a40260 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x78>
 	lea    0x790ac1(%rip),%r9        # 985340 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PackSegmentsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x560>
-	mov    $0x2d0001,%r8d
+	mov    $0x2e0001,%r8d
 	lea    0x778168(%rip),%rcx        
 	movl   $0xb6,(%rsp)
 	call   145ec0 <torch::detail::TorchLibraryInit::TorchLibraryInit(torch::Library::Kind, void (*)(torch::Library&), char const*, c10::optional<c10::DispatchKey>, char const*, unsigned int)@plt>
 	pop    %rax
 	mov    %rbp,%rdi
 	pop    %rdx
 	lea    0x84b9bc(%rip),%rsi        # a40260 <c10::detail::getMaybeFakeTypePtr_<c10::optional<double>, false>::call()::inner_type@@Base+0x78>
@@ -887432,15 +887432,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0xf2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x60(%rsp)
 	jne    5188ea <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0xd5a>
 	movb   $0x1,0x60(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	vmovdqu 0x78(%rsp),%xmm4
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %di,0x62(%rsp)
 	mov    0x60(%rsp),%eax
 	mov    %r15,%rdi
 	lea    0x455a3b(%rip),%rsi        
@@ -887562,15 +887562,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0xf2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x60(%rsp)
 	jne    518beb <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x105b>
 	movb   $0x1,0x60(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	vmovdqu 0x78(%rsp),%xmm7
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %si,0x62(%rsp)
 	mov    0x60(%rsp),%eax
 	mov    %r15,%rdi
 	lea    0x455a42(%rip),%rsi        
@@ -887696,15 +887696,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0xf2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x60(%rsp)
 	jne    518f07 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x1377>
 	movb   $0x1,0x60(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	vmovdqu 0x78(%rsp),%xmm3
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %cx,0x62(%rsp)
 	mov    0x60(%rsp),%eax
 	xor    %ecx,%ecx
 	lea    0x453a8a(%rip),%rsi        
@@ -887783,15 +887783,15 @@
 	lea    0xe8(%rsp),%rax
 	mov    %rax,%rdi
 	mov    %rax,(%rsp)
 	call   14a400 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor)>()@plt>
 	cmpb   $0x0,0xb0(%rsp)
 	jne    519104 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x1574>
 	movb   $0x1,0xb0(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	xor    %ecx,%ecx
 	lea    0x4538b8(%rip),%rsi        
 	mov    %r15,%rdi
 	mov    %dx,0xb2(%rsp)
 	mov    0xb0(%rsp),%eax
 	mov    %r12,%rdx
 	vmovdqu 0xc8(%rsp),%xmm5
@@ -887868,15 +887868,15 @@
 	mov    %rax,0xc8(%rsp)
 	mov    0x5196b7(%rip),%rax        
 	mov    %rax,0xe0(%rsp)
 	call   14a400 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor)>()@plt>
 	cmpb   $0x0,0xb0(%rsp)
 	jne    519308 <int_nbit_split_embedding_uvm_caching_codegen_lookup_function_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, long, long, long, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<long>, c10::optional<at::Tensor>, c10::optional<at::Tensor>, c10::optional<at::Tensor>)@@Base+0x1778>
 	movb   $0x1,0xb0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0xb2(%rsp)
 	mov    0xb0(%rsp),%eax
 	lea    0x4536b5(%rip),%rsi        
 	vmovdqu 0xc8(%rsp),%xmm7
@@ -919564,15 +919564,15 @@
 	mov    0x4fbc5b(%rip),%rax        # a348d8 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, long)@@Base+0x9bc8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14a030 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    538c9c <c10::Dict<std::string, at::Tensor> c10::impl::toTypedDict<std::string, at::Tensor>(c10::Dict<c10::IValue, c10::IValue>)@@Base+0x2b0c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x438ce1(%rip),%rsi        
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -928646,15 +928646,15 @@
 	mov    0x4ef6f7(%rip),%rax        # a31ff0 <typeinfo for void (at::Tensor&, at::Tensor&, at::Tensor&, long, at::Tensor&, c10::optional<at::Tensor> const&, c10::optional<at::Tensor> const&, long)@@Base+0x7290>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14a5e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<void (at::Tensor&, at::Tensor&, at::Tensor&, long, at::Tensor&, c10::optional<at::Tensor> const&, c10::optional<at::Tensor> const&, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    542918 <at::Tensor& std::vector<at::Tensor, std::allocator<at::Tensor> >::emplace_back<at::Tensor&>(at::Tensor&)@@Base+0x2b38>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x42f975(%rip),%rsi        
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -929726,15 +929726,15 @@
 	lea    0x88(%rsp),%rax
 	mov    %rax,%rdi
 	mov    %rax,0x38(%rsp)
 	call   1492e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)>()@plt>
 	cmpb   $0x0,0x50(%rsp)
 	jne    543c00 <fbgemm_gpu::permute_pooled_embs_split_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0xc50>
 	movb   $0x1,0x50(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	mov    0x10(%rsp),%r14
 	mov    0x20(%rsp),%rdi
 	xor    %ecx,%ecx
 	mov    %dx,0x52(%rsp)
 	mov    0x50(%rsp),%eax
 	lea    0x42f0d9(%rip),%rsi        # 972cfa <typeinfo name for void (at::Tensor&, at::Tensor&, at::Tensor&, long, at::Tensor&, c10::optional<at::Tensor> const&, c10::optional<at::Tensor> const&, long)@@Base+0x33a>
 	vmovdqu 0x68(%rsp),%xmm1
@@ -930119,15 +930119,15 @@
 	mov    %rax,0x68(%rsp)
 	mov    0x4ef454(%rip),%rax        
 	mov    %rax,0x80(%rsp)
 	call   1492e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)>()@plt>
 	cmpb   $0x0,0x50(%rsp)
 	jne    54432d <fbgemm_gpu::permute_pooled_embs_split_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x137d>
 	movb   $0x1,0x50(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x68(%rsp),%xmm3
 	vmovdqu 0x78(%rsp),%xmm4
 	xor    %ecx,%ecx
 	mov    %ax,0x52(%rsp)
 	mov    0x50(%rsp),%eax
 	lea    0x42e968(%rip),%rsi        # 972cb8 <typeinfo name for void (at::Tensor&, at::Tensor&, at::Tensor&, long, at::Tensor&, c10::optional<at::Tensor> const&, c10::optional<at::Tensor> const&, long)@@Base+0x2f8>
 	vmovdqu %xmm3,0xb8(%rsp)
@@ -935997,15 +935997,15 @@
 	jae    54a5d7 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x16e7>
 	and    $0x7fff,%edi
 	jne    54a572 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1682>
 	xor    %edx,%edx
 	cmp    $0x9,%ax
 	jne    54a593 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x16a3>
 	movzbl %dl,%eax
-	add    $0x4c,%eax
+	add    $0x4d,%eax
 	ret
 	nopl   (%rax)
 	ret
 	nopl   0x0(%rax)
 	xor    %edx,%edx
 	and    $0x7fff,%edi
 	je     54a581 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1691>
@@ -936018,30 +936018,30 @@
 	cmp    $0x9,%ax
 	je     54a556 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1666>
 	cmp    $0x6,%ax
 	je     54a5c0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x16d0>
 	cmp    $0xc,%ax
 	je     54a5d0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x16e0>
 	movzbl %dl,%edx
-	add    $0x6c,%edx
+	add    $0x6d,%edx
 	cmp    $0x18,%ax
 	mov    $0x0,%eax
 	cmove  %edx,%eax
 	ret
 	nopl   0x0(%rax)
 	movzbl %dl,%eax
-	add    $0x2c,%eax
+	add    $0x2d,%eax
 	ret
 	nopw   0x0(%rax,%rax,1)
 	movzbl %dl,%eax
-	add    $0x3c,%eax
+	add    $0x3d,%eax
 	ret
 	nopw   0x0(%rax,%rax,1)
 	movzbl %dl,%eax
-	add    $0x5c,%eax
+	add    $0x5d,%eax
 	ret
 	ret
 	nopl   0x0(%rax,%rax,1)
 	push   %r12
 	push   %rbx
 	mov    %rdi,%rbx
 	sub    $0x8,%rsp
@@ -941564,27 +941564,27 @@
 	mov    %rax,-0x190(%rbp)
 	movzbl (%r12),%eax
 	test   %al,%al
 	je     5505c0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x76d0>
 	mov    -0x190(%rbp),%rax
 	mov    0x4efc51(%rip),%r15        # a3fa70 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4b0>
 	mov    (%rax),%rax
-	cmpb   $0x0,0xf28(%r15)
+	cmpb   $0x0,0xf48(%r15)
 	mov    0xb8(%rax),%r13
 	je     5503c0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x74d0>
 	mov    %r13,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     54fe56 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x6f66>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%r15,%rax,8),%rax
+	mov    0xed0(%r15,%rax,8),%rax
 	cmpq   $0x0,0x4e4ae2(%rip)        
 	mov    %rax,-0x1b0(%rbp)
 	je     54fe7b <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x6f8b>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4efbf5(%rip),%r15        # a3fa70 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4b0>
 	data16 lea 0x4e37f5(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -941856,15 +941856,15 @@
 	call   147610 <__cxa_atexit@plt>
 	lea    0x4ef6b3(%rip),%rdi        # a3fa60 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4a0>
 	call   149ea0 <__cxa_guard_release@plt>
 	mov    %r15,%rdi
 	call   14a590 <c10::OperatorHandle::~OperatorHandle()@plt>
 	jmp    54fdf6 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x6f06>
 	nop
-	mov    0xea8(%r15),%rax
+	mov    0xec8(%r15),%rax
 	cmpq   $0x0,0x4e4579(%rip)        
 	mov    %rax,-0x1b0(%rbp)
 	je     5503e4 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x74f4>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ef68c(%rip),%r15        # a3fa70 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4b0>
 	data16 lea 0x4e328c(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -942008,15 +942008,15 @@
 	lea    0x4246b1(%rip),%rcx        # 974d60 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1bc0>
 	mov    $0x3f,%edx
 	lea    0x424565(%rip),%rsi        # 974c20 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1a80>
 	lea    0x42690a(%rip),%rdi        # 976fcc <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x1ac>
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4ef399(%rip),%rax        # a3fa70 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4b0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     54fee6 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x6ff6>
 	push   %rbx
 	mov    -0x190(%rbp),%r9
 	mov    %r13,%r8
 	mov    %r12,%rcx
 	push   -0x188(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -942358,20 +942358,20 @@
 	mov    %rax,-0x1b8(%rbp)
 	movzbl (%rax),%eax
 	test   %al,%al
 	je     551100 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x8210>
 	mov    -0x1c8(%rbp),%rax
 	mov    0x4eed44(%rip),%rcx        # a3fa90 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4d0>
 	mov    (%rax),%rax
-	cmpb   $0x0,0xf28(%rcx)
+	cmpb   $0x0,0xf48(%rcx)
 	mov    %rcx,%rdi
 	mov    0xb8(%rax),%rax
 	mov    %rax,-0x1b8(%rbp)
 	jne    550f28 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x8038>
-	mov    0xea8(%rcx),%rax
+	mov    0xec8(%rcx),%rax
 	cmpq   $0x0,0x4e3bcc(%rip)        
 	mov    %rax,-0x1c0(%rbp)
 	je     550d91 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x7ea1>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4eecff(%rip),%rdi        # a3fa90 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4d0>
 	mov    %rdi,-0x1d8(%rbp)
 	data16 lea 0x4e28d8(%rip),%rdi        
@@ -942463,15 +942463,15 @@
 	and    $0x3fff,%eax
 	je     550f44 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x8054>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rcx,%rax,8),%rax
+	mov    0xed0(%rcx,%rax,8),%rax
 	cmpq   $0x0,0x4e39f4(%rip)        
 	mov    %rax,-0x1c0(%rbp)
 	je     550f69 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x8079>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4eeb27(%rip),%rcx        # a3fa90 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4d0>
 	mov    %rcx,-0x1d8(%rbp)
 	data16 lea 0x4e2700(%rip),%rdi        
@@ -942595,15 +942595,15 @@
 	mov    0x4e2dc5(%rip),%rax        
 	mov    %r8,(%rax)
 	mov    %rax,-0x1d8(%rbp)
 	call   149ea0 <__cxa_guard_release@plt>
 	mov    -0x1d8(%rbp),%rax
 	jmp    550ff0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x8100>
 	mov    0x4ee8ab(%rip),%rdx        # a3fa90 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x4d0>
-	cmpb   $0x0,0xfa8(%rdx)
+	cmpb   $0x0,0xfc8(%rdx)
 	je     550e19 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x7f29>
 	push   %r15
 	vmovsd -0x1d0(%rbp),%xmm0
 	mov    %rax,%r8
 	mov    %r14,%rdi
 	push   %rbx
 	mov    -0x1c8(%rbp),%r9
@@ -944134,18 +944134,18 @@
 	mov    -0x140(%rbp),%r14
 	mov    %rax,%r15
 	movzbl (%rax),%eax
 	test   %al,%al
 	je     5537b0 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1700>
 	mov    0x4eca3c(%rip),%r15        # a3fa30 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x470>
 	mov    (%r14),%rax
-	cmpb   $0x0,0xf28(%r15)
+	cmpb   $0x0,0xf48(%r15)
 	mov    0xb8(%rax),%rbx
 	jne    553430 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1380>
-	mov    0xea8(%r15),%rax
+	mov    0xec8(%r15),%rax
 	cmpq   $0x0,0x4e192d(%rip)        
 	mov    %rax,-0x188(%rbp)
 	je     553030 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xf80>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4eca00(%rip),%r15        # a3fa30 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x470>
 	data16 lea 0x4e0640(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -944360,15 +944360,15 @@
 	and    $0x3fff,%eax
 	je     55344f <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x139f>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%r15,%rax,8),%rax
+	mov    0xed0(%r15,%rax,8),%rax
 	cmpq   $0x0,0x4e14e9(%rip)        
 	mov    %rax,-0x188(%rbp)
 	je     553474 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x13c4>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ec5bc(%rip),%r15        # a3fa30 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x470>
 	data16 lea 0x4e01fc(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -944611,15 +944611,15 @@
 	lea    0x4236ca(%rip),%rdi        # 976fcc <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x1ac>
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	xor    %eax,%eax
 	jmp    552fb5 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xf05>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4ec109(%rip),%rax        # a3fa30 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x470>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55309e <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xfee>
 	push   %r12
 	mov    -0x190(%rbp),%rdi
 	vxorpd %xmm0,%xmm0,%xmm0
 	mov    %r14,%r9
 	push   -0x1b0(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -944955,18 +944955,18 @@
 	mov    -0x140(%rbp),%r15
 	mov    %rax,%r14
 	movzbl (%rax),%eax
 	test   %al,%al
 	je     554820 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2770>
 	mov    0x4eb9ec(%rip),%r14        # a3f970 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3b0>
 	mov    (%r15),%rax
-	cmpb   $0x0,0xf28(%r14)
+	cmpb   $0x0,0xf48(%r14)
 	mov    0xb8(%rax),%rbx
 	jne    554138 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2088>
-	mov    0xea8(%r14),%rax
+	mov    0xec8(%r14),%rax
 	cmpq   $0x0,0x4e099d(%rip)        
 	mov    %rax,-0x188(%rbp)
 	je     553fc0 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1f10>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4eb9b0(%rip),%r14        # a3f970 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3b0>
 	data16 lea 0x4df6b0(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -945048,15 +945048,15 @@
 	and    $0x3fff,%eax
 	je     554157 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x20a7>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%r14,%rax,8),%rax
+	mov    0xed0(%r14,%rax,8),%rax
 	cmpq   $0x0,0x4e07e1(%rip)        
 	mov    %rax,-0x188(%rbp)
 	je     55417c <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x20cc>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4eb7f4(%rip),%r14        # a3f970 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3b0>
 	data16 lea 0x4df4f4(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -945469,15 +945469,15 @@
 	nop
 	mov    (%rdi),%rax
 	call   *0x78(%rax)
 	mov    %rax,%rbx
 	jmp    5540c1 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2011>
 	xchg   %ax,%ax
 	mov    0x4eb009(%rip),%rax        # a3f970 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3b0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55402e <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1f7e>
 	push   %r13
 	lea    -0x98(%rbp),%rax
 	vxorpd %xmm0,%xmm0,%xmm0
 	mov    %r15,%r9
 	push   -0x1b8(%rbp)
 	mov    %rbx,%r8
@@ -945985,26 +945985,26 @@
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%r13
 	or     0xb8(%rax),%r13
 	mov    -0x1b0(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r13
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     5558e8 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3838>
 	mov    %r13,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     55542a <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x337a>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4df50e(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     55544f <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x339f>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ea601(%rip),%rdi        # a3fa50 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x490>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4de21a(%rip),%rdi        
@@ -946235,15 +946235,15 @@
 	call   54c6b0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x37c0>
 	jmp    55506a <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2fba>
 	mov    $0x4,%esi
 	mov    %r13,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    554fd7 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2f27>
 	nopw   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4df051(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     55590c <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x385c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ea144(%rip),%rdi        # a3fa50 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x490>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4ddd5d(%rip),%rdi        
@@ -946345,15 +946345,15 @@
 	jmp    5550ad <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2ffd>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	jne    555870 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x37c0>
 	jmp    5557c8 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3718>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4e9f29(%rip),%rax        # a3fa50 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x490>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     5554c4 <fbgemm_gpu::jagged_dense_elementwise_add(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3414>
 	sub    $0x8,%rsp
 	push   -0x1b8(%rbp)
 	mov    -0x1b0(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1a8(%rbp)
 	mov    %r13,%rcx
@@ -946747,27 +946747,27 @@
 	mov    0x4e97b4(%rip),%rdi        # a3f9f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x430>
 	mov    0xb8(%rax),%rax
 	mov    %rax,%rsi
 	mov    -0x188(%rbp),%rax
 	or     0xb8(%rax),%rsi
 	mov    0x0(%r13),%rax
 	or     0xb8(%rax),%rsi
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	mov    %rsi,-0x198(%rbp)
 	mov    %rsi,%rax
 	je     556895 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xb95>
 	shr    %rax
 	and    $0x3fff,%eax
 	je     556292 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x592>
 	bsr    %rax,%rax
 	mov    $0x40,%edx
 	xor    $0x3f,%rax
 	sub    %eax,%edx
 	movzbl %dl,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4de6a6(%rip)        
 	mov    %rax,-0x1a0(%rbp)
 	je     5562b7 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x5b7>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e9739(%rip),%rdi        # a3f9f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x430>
 	mov    %rdi,-0x1d8(%rbp)
 	movabs $0x1008000000,%r12
@@ -947071,15 +947071,15 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	pop    %rbp
 	ret
 	cmpq   $0x0,0x4de0ab(%rip)        
-	mov    0xea8(%rdi),%r12
+	mov    0xec8(%rdi),%r12
 	je     5568b2 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xbb2>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e913e(%rip),%rdi        # a3f9f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x430>
 	mov    %rdi,-0x1a0(%rbp)
 	data16 lea 0x4dcdb7(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
 	mov    -0x1a0(%rbp),%rdi
@@ -947170,15 +947170,15 @@
 	mov    %rax,-0x1a0(%rbp)
 	lea    -0x180(%rbp),%rax
 	push   %rax
 	mov    %rax,-0x1d8(%rbp)
 	call   145af0 <c10::impl::BoxedKernelWrapper<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@plt>
 	jmp    55638a <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x68a>
 	mov    0x4e8f5d(%rip),%rax        # a3f9f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x430>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     556335 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x635>
 	sub    $0x8,%rsp
 	lea    -0x188(%rbp),%rax
 	lea    -0x170(%rbp),%r12
 	mov    -0x1e0(%rbp),%r8
 	push   %rax
 	mov    -0x198(%rbp),%rcx
@@ -947653,26 +947653,26 @@
 	mov    -0x1a8(%rbp),%rax
 	mov    0x4e85bc(%rip),%rdi        # a3fa10 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x450>
 	mov    (%rax),%rdx
 	mov    -0x1b0(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%rbx
 	or     0xb8(%rax),%rbx
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     557988 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1c88>
 	mov    %rbx,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     55749b <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x179b>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4dd49d(%rip)        
 	mov    %rax,-0x1f0(%rbp)
 	je     5574c0 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x17c0>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e8550(%rip),%rdi        # a3fa10 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x450>
 	mov    %rdi,-0x1f8(%rbp)
 	movabs $0x1008000000,%r12
@@ -947907,15 +947907,15 @@
 	lock addl $0x1,(%rax)
 	jmp    55713d <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x143d>
 	mov    $0x3,%esi
 	mov    %r12,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    5570a8 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x13a8>
 	nopw   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4dcfb1(%rip)        
 	mov    %rax,-0x1f0(%rbp)
 	je     5579ac <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1cac>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e8064(%rip),%rdi        # a3fa10 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x450>
 	mov    %rdi,-0x1f8(%rbp)
 	movabs $0xffffc1ffffffffff,%r12
@@ -948184,15 +948184,15 @@
 	jmp    557af0 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1df0>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1b9(%rbp)
 	je     55783c <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1b3c>
 	jmp    5578f0 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1bf0>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4e7b61(%rip),%rax        # a3fa10 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x450>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     557533 <fbgemm_gpu::jagged_dense_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1833>
 	push   -0x1b0(%rbp)
 	lea    -0x120(%rbp),%rbx
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1c8(%rbp)
 	mov    %r12,%rcx
@@ -948490,28 +948490,28 @@
 	mov    %rax,%rcx
 	mov    -0x168(%rbp),%rax
 	or     0xb8(%rax),%rcx
 	mov    -0x160(%rbp),%rax
 	or     0xb8(%rax),%rcx
 	mov    (%r12),%rax
 	or     0xb8(%rax),%rcx
-	cmpb   $0x0,0xf28(%r14)
+	cmpb   $0x0,0xf48(%r14)
 	mov    %rcx,-0x178(%rbp)
 	mov    %rcx,%rax
 	je     5588c0 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x7a0>
 	shr    %rax
 	and    $0x3fff,%eax
 	je     558432 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x312>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
 	cmpq   $0x0,0x4dc50e(%rip)        
-	mov    0xeb0(%r14,%rax,8),%r13
+	mov    0xed0(%r14,%rax,8),%r13
 	je     558450 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x330>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e7560(%rip),%r14        # a3f9b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3f0>
 	data16 lea 0x4db220(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
 	mov    %rax,%rdx
 	movabs $0x1008000000,%rax
@@ -948736,15 +948736,15 @@
 	mov    0x4db6dc(%rip),%rdx        
 	mov    %r14,%rdi
 	mov    %rax,(%rdx)
 	call   149ea0 <__cxa_guard_release@plt>
 	jmp    5583bf <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x29f>
 	nopl   0x0(%rax)
 	cmpq   $0x0,0x4dc080(%rip)        
-	mov    0xea8(%r14),%r13
+	mov    0xec8(%r14),%r13
 	je     5588dd <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x7bd>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e70d3(%rip),%r14        # a3f9b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3f0>
 	data16 lea 0x4dad93(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
 	mov    %rax,%rdx
 	movabs $0xffffc1ffffffffff,%rax
@@ -948920,15 +948920,15 @@
 	lea    0x41c099(%rip),%rcx        # 974cc0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1b20>
 	mov    $0xf1,%edx
 	lea    0x41bfed(%rip),%rsi        # 974c20 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1a80>
 	lea    0x41e392(%rip),%rdi        # 976fcc <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x1ac>
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	mov    0x4e6d69(%rip),%rax        # a3f9b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3f0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     5584cb <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3ab>
 	sub    $0x8,%rsp
 	lea    -0x160(%rbp),%rax
 	lea    -0x168(%rbp),%r14
 	mov    -0x1c0(%rbp),%r8
 	push   %rax
 	mov    -0x178(%rbp),%rcx
@@ -949513,26 +949513,26 @@
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%r13
 	or     0xb8(%rax),%r13
 	mov    -0x1a8(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r13
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     559e68 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1d48>
 	mov    %r13,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     5598d0 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x17b0>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4db068(%rip)        
 	mov    %rax,-0x1d8(%rbp)
 	je     5598f5 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x17d5>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e60db(%rip),%rdi        # a3f9d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x410>
 	mov    %rdi,-0x1f8(%rbp)
 	data16 lea 0x4d9d74(%rip),%rdi        
@@ -949800,15 +949800,15 @@
 	lock addl $0x1,(%rax)
 	jmp    559567 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1447>
 	mov    $0x3,%esi
 	mov    %r13,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    5594c3 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x13a3>
 	nopw   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4daad1(%rip)        
 	mov    %rax,-0x1d8(%rbp)
 	je     559e8c <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1d6c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e5b44(%rip),%rdi        # a3f9d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x410>
 	mov    %rdi,-0x1f8(%rbp)
 	data16 lea 0x4d97dd(%rip),%rdi        
@@ -949859,15 +949859,15 @@
 	jmp    559588 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1468>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c1(%rbp)
 	jne    559dd0 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1cb0>
 	jmp    559c6d <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1b4d>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4e5a31(%rip),%rax        # a3f9d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x410>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     559971 <fbgemm_gpu::jagged_dense_elementwise_mul(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1851>
 	push   -0x1b8(%rbp)
 	lea    -0xe0(%rbp),%r13
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b0(%rbp)
 	lea    0x4e59fc(%rip),%rsi        # a3f9d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x410>
@@ -950092,28 +950092,28 @@
 	je     55a5b8 <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x458>
 	mov    0x4d7a83(%rip),%r15        
 	movzbl (%r15),%eax
 	test   %al,%al
 	je     55a688 <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x528>
 	mov    0x4e5610(%rip),%rcx        # a3f990 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3d0>
 	mov    (%r14),%rax
-	cmpb   $0x0,0xf28(%rcx)
+	cmpb   $0x0,0xf48(%rcx)
 	mov    0xb8(%rax),%r15
 	mov    %rcx,%rdi
 	je     55a538 <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x3d8>
 	mov    %r15,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     55a3b9 <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x259>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rcx,%rax,8),%rax
+	mov    0xed0(%rcx,%rax,8),%rax
 	cmpq   $0x0,0x4da57f(%rip)        
 	mov    %rax,-0xc0(%rbp)
 	je     55a3de <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x27e>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e55b2(%rip),%rcx        # a3f990 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3d0>
 	mov    %rcx,-0xd0(%rbp)
 	data16 lea 0x4d928b(%rip),%rdi        
@@ -950185,15 +950185,15 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	pop    %rbp
 	ret
 	nopl   0x0(%rax,%rax,1)
-	mov    0xea8(%rcx),%rax
+	mov    0xec8(%rcx),%rax
 	cmpq   $0x0,0x4da401(%rip)        
 	mov    %rax,-0xc0(%rbp)
 	je     55a55c <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x3fc>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e5434(%rip),%rdi        # a3f990 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3d0>
 	mov    %rdi,-0xd0(%rbp)
 	data16 lea 0x4d910d(%rip),%rdi        
@@ -950271,15 +950271,15 @@
 	mov    %r13,%rdi
 	call   146ec0 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<c10::SymInt> const&), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::optional<c10::SymInt> const&)@plt>
 	pop    %rax
 	pop    %rdx
 	jmp    55a485 <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x325>
 	nopl   0x0(%rax)
 	mov    0x4e5291(%rip),%rdx        # a3f990 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x3d0>
-	cmpb   $0x0,0xfa8(%rdx)
+	cmpb   $0x0,0xfc8(%rdx)
 	je     55a45f <fbgemm_gpu::batched_dense_vec_jagged_2d_mul(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x2ff>
 	push   -0xc8(%rbp)
 	mov    %r14,%r9
 	mov    %rax,%r8
 	mov    %r15,%rcx
 	push   %rbx
 	lea    -0x98(%rbp),%rdx
@@ -951610,27 +951610,27 @@
 	mov    0x4e3760(%rip),%r15        # a3f930 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x370>
 	mov    0xb8(%rax),%rcx
 	mov    -0x158(%rbp),%rax
 	or     0xb8(%rax),%rcx
 	mov    -0x168(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%rcx
-	cmpb   $0x0,0xf28(%r15)
+	cmpb   $0x0,0xf48(%r15)
 	mov    %rcx,-0x1a8(%rbp)
 	mov    %rcx,%rax
 	je     55c7d8 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x14e8>
 	shr    %rax
 	and    $0x3fff,%eax
 	je     55c22a <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xf3a>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%r15,%rax,8),%rax
+	mov    0xed0(%r15,%rax,8),%rax
 	cmpq   $0x0,0x4d870e(%rip)        
 	mov    %rax,-0x1b0(%rbp)
 	je     55c24f <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xf5f>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e36e1(%rip),%r15        # a3f930 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x370>
 	data16 lea 0x4d7421(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -951914,15 +951914,15 @@
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	pop    %rbp
 	ret
 	nopl   0x0(%rax,%rax,1)
-	mov    0xea8(%r15),%rax
+	mov    0xec8(%r15),%rax
 	cmpq   $0x0,0x4d8161(%rip)        
 	mov    %rax,-0x1b0(%rbp)
 	je     55c7fc <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x150c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e3134(%rip),%r15        # a3f930 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x370>
 	data16 lea 0x4d6e74(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -952026,15 +952026,15 @@
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    -0x148(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    55c177 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe87>
 	nopl   0x0(%rax)
 	mov    0x4e2f01(%rip),%rax        # a3f930 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x370>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55c2bb <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xfcb>
 	sub    $0x8,%rsp
 	push   -0x1a0(%rbp)
 	lea    -0x158(%rbp),%rax
 	lea    -0x150(%rbp),%r15
 	push   %rax
 	lea    -0x98(%rbp),%rdx
@@ -952314,15 +952314,15 @@
 	je     55d710 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2420>
 	mov    0x4e2962(%rip),%rax        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
 	lea    -0x160(%rbp),%r14
 	mov    -0x178(%rbp),%rcx
 	lea    -0x168(%rbp),%rsi
 	mov    %r14,%rdx
 	mov    %rsi,-0x1a0(%rbp)
-	lea    0xea0(%rax),%rdi
+	lea    0xec0(%rax),%rdi
 	call   549fa0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x10b0>
 	mov    0x4e2930(%rip),%rdi        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
 	mov    %rax,%rsi
 	mov    %rax,%r12
 	call   146e30 <c10::impl::OperatorEntry::lookup(c10::DispatchKeySet) const@plt>
 	xor    %esi,%esi
 	mov    %r15,%rdi
@@ -952357,15 +952357,15 @@
 	test   %al,%al
 	je     55d6e0 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x23f0>
 	mov    0x4e2882(%rip),%rax        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
 	lea    -0x170(%rbp),%r13
 	mov    -0x1a8(%rbp),%rcx
 	mov    %r14,%rdx
 	mov    %r13,%rsi
-	lea    0xea0(%rax),%rdi
+	lea    0xec0(%rax),%rdi
 	call   549fa0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x10b0>
 	mov    0x4e285b(%rip),%rdi        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
 	mov    %rax,%rsi
 	mov    %rax,%r12
 	call   146e30 <c10::impl::OperatorEntry::lookup(c10::DispatchKeySet) const@plt>
 	xor    %esi,%esi
 	mov    %r15,%rdi
@@ -952751,15 +952751,15 @@
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nop
 	lea    -0x148(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    55cf2f <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1c3f>
 	nopl   0x0(%rax)
 	mov    0x4e2101(%rip),%rax        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55cfe9 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1cf9>
 	sub    $0x8,%rsp
 	push   -0x198(%rbp)
 	lea    -0x158(%rbp),%rax
 	mov    -0x1a0(%rbp),%r9
 	push   -0x178(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -952770,15 +952770,15 @@
 	lea    0x4e20b9(%rip),%rsi        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
 	mov    %rax,-0x1d0(%rbp)
 	call   147180 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@plt>
 	add    $0x20,%rsp
 	jmp    55d033 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1d43>
 	nopl   0x0(%rax)
 	mov    0x4e2099(%rip),%rax        # a3f8f0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x330>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55d0be <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1dce>
 	sub    $0x8,%rsp
 	push   -0x198(%rbp)
 	lea    -0x150(%rbp),%rax
 	mov    -0x1c8(%rbp),%r8
 	push   -0x1a8(%rbp)
 	mov    %r13,%r9
@@ -953330,26 +953330,26 @@
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%r13
 	or     0xb8(%rax),%r13
 	mov    -0x1a8(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r13
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     55e9a8 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x36b8>
 	mov    %r13,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     55e427 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3137>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4d6511(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     55e44c <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x315c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e14c4(%rip),%rdi        # a3f910 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x350>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4d521d(%rip),%rdi        
@@ -953615,15 +953615,15 @@
 	call   54c6b0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x37c0>
 	jmp    55df9a <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2caa>
 	mov    $0x4,%esi
 	mov    %r13,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    55df07 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2c17>
 	nopw   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4d5f91(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     55e9cc <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x36dc>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4e0f44(%rip),%rdi        # a3f910 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x350>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4d4c9d(%rip),%rdi        
@@ -953689,15 +953689,15 @@
 	jmp    55dfdd <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x2ced>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	jne    55e930 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x3640>
 	jmp    55e7c6 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x34d6>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4e0dd9(%rip),%rax        # a3f910 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x350>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55e4c1 <fbgemm_gpu::jagged_dense_elementwise_add_jagged_output(at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x31d1>
 	sub    $0x8,%rsp
 	push   -0x1e8(%rbp)
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b8(%rbp)
 	mov    %r13,%rcx
@@ -953965,15 +953965,15 @@
 	test   %al,%al
 	je     55f830 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xb30>
 	mov    0x4e08a8(%rip),%rax        # a3f8b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2f0>
 	lea    -0x170(%rbp),%r12
 	mov    -0x1b0(%rbp),%rsi
 	mov    %r14,%rcx
 	mov    %r12,%rdx
-	lea    0xea0(%rax),%rdi
+	lea    0xec0(%rax),%rdi
 	call   549fa0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x10b0>
 	mov    0x4e0881(%rip),%rdi        # a3f8b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2f0>
 	mov    %rax,%rsi
 	mov    %rax,-0x1e0(%rbp)
 	call   146e30 <c10::impl::OperatorEntry::lookup(c10::DispatchKeySet) const@plt>
 	xor    %esi,%esi
 	mov    %r13,%rdi
@@ -954016,15 +954016,15 @@
 	test   %al,%al
 	je     55f860 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xb60>
 	mov    0x4e0791(%rip),%rax        # a3f890 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2d0>
 	lea    -0x178(%rbp),%r15
 	mov    -0x1b0(%rbp),%rdx
 	mov    %r12,%rcx
 	mov    %r15,%rsi
-	lea    0xea0(%rax),%rdi
+	lea    0xec0(%rax),%rdi
 	call   549fa0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x10b0>
 	mov    0x4e076a(%rip),%rdi        # a3f890 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2d0>
 	mov    %rax,%rsi
 	mov    %rax,-0x1e8(%rbp)
 	call   146e30 <c10::impl::OperatorEntry::lookup(c10::DispatchKeySet) const@plt>
 	xor    %esi,%esi
 	mov    %r13,%rdi
@@ -954439,15 +954439,15 @@
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopl   (%rax)
 	lea    -0x148(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    55ef96 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x296>
 	nopl   0x0(%rax)
 	mov    0x4dff41(%rip),%rax        # a3f890 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2d0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55f153 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x453>
 	sub    $0x8,%rsp
 	push   -0x188(%rbp)
 	lea    -0x158(%rbp),%rax
 	mov    -0x1d0(%rbp),%r8
 	push   %r12
 	lea    -0x98(%rbp),%rdx
@@ -954458,15 +954458,15 @@
 	lea    0x4dfef9(%rip),%rsi        # a3f890 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2d0>
 	mov    %rax,-0x1e0(%rbp)
 	call   147180 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@plt>
 	add    $0x20,%rsp
 	jmp    55f19d <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x49d>
 	nopl   0x0(%rax)
 	mov    0x4dfef9(%rip),%rax        # a3f8b0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2f0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     55f05c <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x35c>
 	sub    $0x8,%rsp
 	push   -0x188(%rbp)
 	lea    -0x160(%rbp),%rax
 	mov    -0x1b0(%rbp),%r9
 	push   %r14
 	lea    -0x98(%rbp),%rdx
@@ -955036,26 +955036,26 @@
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%r13
 	or     0xb8(%rax),%r13
 	mov    -0x1a8(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r13
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     560b68 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1e68>
 	mov    %r13,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     5605e7 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x18e7>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4d4351(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     56060c <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x190c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4df2c4(%rip),%rdi        # a3f8d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x310>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4d305d(%rip),%rdi        
@@ -955321,15 +955321,15 @@
 	call   54c6b0 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x37c0>
 	jmp    56015a <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x145a>
 	mov    $0x4,%esi
 	mov    %r13,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    5600c7 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x13c7>
 	nopw   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4d3dd1(%rip)        
 	mov    %rax,-0x200(%rbp)
 	je     560b8c <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1e8c>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ded44(%rip),%rdi        # a3f8d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x310>
 	mov    %rdi,-0x208(%rbp)
 	data16 lea 0x4d2add(%rip),%rdi        
@@ -955395,15 +955395,15 @@
 	jmp    56019d <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x149d>
 	nopl   0x0(%rax)
 	cmpb   $0x0,-0x1c9(%rbp)
 	jne    560af0 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1df0>
 	jmp    560986 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1c86>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4debd9(%rip),%rax        # a3f8d0 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x310>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     560681 <fbgemm_gpu::jagged_jagged_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1981>
 	sub    $0x8,%rsp
 	push   -0x1e8(%rbp)
 	mov    -0x1a8(%rbp),%r9
 	lea    -0x98(%rbp),%rdx
 	push   -0x1b8(%rbp)
 	mov    %r13,%rcx
@@ -955812,27 +955812,27 @@
 	mov    -0x1b0(%rbp),%rax
 	mov    0x4de3f9(%rip),%rdi        # a3f950 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x390>
 	mov    (%rax),%rdx
 	mov    -0x1a8(%rbp),%rax
 	mov    (%rax),%rax
 	mov    0xb8(%rdx),%r14
 	or     0xb8(%rax),%r14
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     561ca8 <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xde8>
 	mov    %r14,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     56159e <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x6de>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
 	cmpq   $0x0,0x4d33a2(%rip)        
-	mov    0xeb0(%rdi,%rax,8),%rbx
+	mov    0xed0(%rdi,%rax,8),%rbx
 	je     5615bc <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x6fc>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4de394(%rip),%rdi        # a3f950 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x390>
 	mov    %rdi,-0x1e8(%rbp)
 	movabs $0x1008000000,%r13
 	data16 lea 0x4d20a3(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -956170,15 +956170,15 @@
 	jmp    561348 <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x488>
 	mov    $0x3,%esi
 	mov    %r13,%rdi
 	call   149590 <std::vector<bool, std::allocator<bool> >::_M_reallocate(unsigned long)@plt>
 	jmp    5612b3 <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x3f3>
 	nopw   0x0(%rax,%rax,1)
 	cmpq   $0x0,0x4d2c98(%rip)        
-	mov    0xea8(%rdi),%rbx
+	mov    0xec8(%rdi),%rbx
 	je     561cc5 <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xe05>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4ddc8b(%rip),%rdi        # a3f950 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x390>
 	mov    %rdi,-0x1e8(%rbp)
 	movabs $0xffffc1ffffffffff,%r13
 	data16 lea 0x4d199a(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -956228,15 +956228,15 @@
 	jmp    561a9c <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xbdc>
 	nopw   0x0(%rax,%rax,1)
 	lea    -0x120(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    5617fe <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x93e>
 	nopl   0x0(%rax)
 	mov    0x4ddb69(%rip),%rax        # a3f950 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x390>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     561627 <fbgemm_gpu::jagged_dense_bmm(at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x767>
 	push   -0x1d0(%rbp)
 	mov    %rbx,%r8
 	mov    %r13,%rcx
 	lea    -0xe0(%rbp),%r14
 	push   -0x1a8(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -956542,26 +956542,26 @@
 	mov    0xb8(%rax),%r15
 	mov    -0x178(%rbp),%rax
 	or     0xb8(%rax),%r15
 	mov    -0x170(%rbp),%rax
 	or     0xb8(%rax),%r15
 	mov    -0x168(%rbp),%rax
 	or     0xb8(%rax),%r15
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     562a30 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0xa90>
 	mov    %r15,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     5623b7 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x417>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4d2581(%rip)        
 	mov    %rax,-0x1d0(%rbp)
 	je     5623ea <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x44a>
 	lea    -0x178(%rbp),%rax
 	mov    %rax,-0x190(%rbp)
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4dd466(%rip),%rdi        # a3f850 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x290>
@@ -956884,15 +956884,15 @@
 	mov    -0x198(%rbp),%rdi
 	mov    %r13,%rsi
 	call   146b70 <at::Tensor& std::vector<at::Tensor, std::allocator<at::Tensor> >::emplace_back<at::Tensor>(at::Tensor&&)@plt>
 	mov    %r13,%rdi
 	call   1453b0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	jmp    5629c4 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0xa24>
 	nopl   0x0(%rax)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4d1f09(%rip)        
 	mov    %rax,-0x1d0(%rbp)
 	je     562a62 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0xac2>
 	lea    -0x178(%rbp),%rax
 	mov    %rax,-0x190(%rbp)
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4dcdee(%rip),%rdi        # a3f850 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x290>
@@ -957035,15 +957035,15 @@
 	lea    0x40b0f1(%rip),%rcx        
 	mov    $0x287,%edx
 	lea    0x40b195(%rip),%rsi        
 	lea    0x409c2a(%rip),%rdi        
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4dcaf9(%rip),%rax        # a3f850 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x290>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     562479 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x4d9>
 	sub    $0x8,%rsp
 	push   -0x1e0(%rbp)
 	lea    -0x168(%rbp),%rax
 	lea    -0x160(%rbp),%r15
 	push   -0x1c8(%rbp)
 	mov    %r15,%r9
@@ -957711,26 +957711,26 @@
 	or     0xb8(%rax),%r14
 	mov    -0x1b0(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r14
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rax
 	or     0xb8(%rax),%r14
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	je     564240 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x22a0>
 	mov    %r14,%rax
 	shr    %rax
 	and    $0x3fff,%eax
 	je     563bc0 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x1c20>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4d0d78(%rip)        
 	mov    %rax,-0x218(%rbp)
 	je     563be5 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x1c45>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4dbc8b(%rip),%rdi        # a3f870 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2b0>
 	mov    %rdi,-0x220(%rbp)
 	movabs $0x1008000000,%r13
@@ -958036,15 +958036,15 @@
 	mov    (%rdi),%rax
 	call   *0x60(%rax)
 	jmp    5636c8 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x1728>
 	nopl   0x0(%rax,%rax,1)
 	lock addl $0x1,0xc(%r15)
 	jmp    5634fc <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x155c>
 	nopl   0x0(%rax,%rax,1)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4d06f9(%rip)        
 	mov    %rax,-0x218(%rbp)
 	je     564264 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x22c4>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4db60c(%rip),%rdi        # a3f870 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2b0>
 	mov    %rdi,-0x220(%rbp)
 	movabs $0xffffc1ffffffffff,%r13
@@ -958182,15 +958182,15 @@
 	jmp    5640f0 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x2150>
 	lea    0x4079dd(%rip),%rcx        # 96bf04 <asmjit::_abi_1_9::FuncSignatureT<int, int, unsigned long, float*, float const*, float*, long const*, float, float, int const*, float, double const*, long>::FuncSignatureT(asmjit::_abi_1_9::CallConvId, unsigned int)::ret_args@@Base+0xac4>
 	mov    $0x4cc,%edx
 	lea    0x407a05(%rip),%rsi        # 96bf38 <asmjit::_abi_1_9::FuncSignatureT<int, int, unsigned long, float*, float const*, float*, long const*, float, float, int const*, float, double const*, long>::FuncSignatureT(asmjit::_abi_1_9::CallConvId, unsigned int)::ret_args@@Base+0xaf8>
 	lea    0x4079e8(%rip),%rdi        # 96bf22 <asmjit::_abi_1_9::FuncSignatureT<int, int, unsigned long, float*, float const*, float*, long const*, float, float, int const*, float, double const*, long>::FuncSignatureT(asmjit::_abi_1_9::CallConvId, unsigned int)::ret_args@@Base+0xae2>
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	mov    0x4db32a(%rip),%rax        # a3f870 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x2b0>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     563c58 <fbgemm_gpu::jagged_softmax(at::Tensor const&, at::Tensor const&, long)@@Base+0x1cb8>
 	push   -0x208(%rbp)
 	mov    %r14,%r8
 	mov    %r13,%rcx
 	mov    -0x1b8(%rbp),%r9
 	push   -0x1d8(%rbp)
 	lea    -0x98(%rbp),%rdx
@@ -958489,27 +958489,27 @@
 	or     0xb8(%rax),%rcx
 	mov    -0x168(%rbp),%rax
 	or     0xb8(%rax),%rcx
 	mov    -0x180(%rbp),%rax
 	or     0xb8(%rax),%rcx
 	mov    -0x170(%rbp),%rax
 	or     0xb8(%rax),%rcx
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	mov    %rcx,-0x198(%rbp)
 	mov    %rcx,%rax
 	je     5651a0 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x9d0>
 	shr    %rax
 	and    $0x3fff,%eax
 	je     564b39 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x369>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
-	mov    0xeb0(%rdi,%rax,8),%rax
+	mov    0xed0(%rdi,%rax,8),%rax
 	cmpq   $0x0,0x4cfdff(%rip)        
 	mov    %rax,-0x1d0(%rbp)
 	je     564b65 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x395>
 	lea    -0x180(%rbp),%r14
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4dacab(%rip),%rdi        # a3f810 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x250>
 	mov    %rdi,-0x1d8(%rbp)
@@ -958832,15 +958832,15 @@
 	mov    -0x190(%rbp),%rdi
 	mov    %r15,%rsi
 	call   146b70 <at::Tensor& std::vector<at::Tensor, std::allocator<at::Tensor> >::emplace_back<at::Tensor>(at::Tensor&&)@plt>
 	mov    %r15,%rdi
 	call   1453b0 <c10::intrusive_ptr<c10::TensorImpl, c10::UndefinedTensorImpl>::reset_()@plt>
 	jmp    56513c <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x96c>
 	nopl   0x0(%rax)
-	mov    0xea8(%rdi),%rax
+	mov    0xec8(%rdi),%rax
 	cmpq   $0x0,0x4cf799(%rip)        
 	mov    %rax,-0x1d0(%rbp)
 	je     5651cb <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x9fb>
 	lea    -0x180(%rbp),%r14
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4da645(%rip),%rdi        # a3f810 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x250>
 	mov    %rdi,-0x1d8(%rbp)
@@ -958979,15 +958979,15 @@
 	lea    0x408991(%rip),%rcx        
 	mov    $0x287,%edx
 	lea    0x408a35(%rip),%rsi        
 	lea    0x4074ca(%rip),%rdi        
 	call   145e50 <c10::detail::torchCheckFail(char const*, char const*, unsigned int, char const*)@plt>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x4da359(%rip),%rax        # a3f810 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x250>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     564be3 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x413>
 	sub    $0x8,%rsp
 	lea    -0x170(%rbp),%rax
 	lea    -0x180(%rbp),%r14
 	mov    -0x1d0(%rbp),%r8
 	push   $0x1
 	lea    -0x160(%rbp),%r9
@@ -959713,27 +959713,27 @@
 	mov    -0x2a0(%rbp),%rsi
 	or     0xb8(%rdx),%rax
 	mov    (%rsi),%rdx
 	mov    -0x2b0(%rbp),%rsi
 	or     0xb8(%rdx),%rax
 	mov    (%rsi),%rdx
 	or     0xb8(%rdx),%rax
-	cmpb   $0x0,0xf28(%rdi)
+	cmpb   $0x0,0xf48(%rdi)
 	mov    %rax,-0x318(%rbp)
 	je     566af0 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x2320>
 	shr    %rax
 	and    $0x3fff,%eax
 	je     56640c <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x1c3c>
 	bsr    %rax,%rdx
 	mov    $0x40,%eax
 	xor    $0x3f,%rdx
 	sub    %edx,%eax
 	movzbl %al,%eax
 	cmpq   $0x0,0x4ce534(%rip)        
-	mov    0xeb0(%rdi,%rax,8),%rbx
+	mov    0xed0(%rdi,%rax,8),%rbx
 	je     56642a <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x1c5a>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4d9406(%rip),%rdi        # a3f830 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x270>
 	mov    %rdi,-0x320(%rbp)
 	movabs $0x1008000000,%r13
 	data16 lea 0x4cd235(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -960066,15 +960066,15 @@
 	jmp    565c9d <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x14cd>
 	nopl   0x0(%rax)
 	mov    -0x308(%rbp),%rax
 	lock addl $0x1,(%rax)
 	jmp    565c7c <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x14ac>
 	nopl   0x0(%rax,%rax,1)
 	cmpq   $0x0,0x4cde50(%rip)        
-	mov    0xea8(%rdi),%rbx
+	mov    0xec8(%rdi),%rbx
 	je     566b0d <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x233d>
 	call   14be70 <TLS init function for c10::impl::raw_local_dispatch_key_set@plt>
 	mov    0x4d8d23(%rip),%rdi        # a3f830 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x270>
 	mov    %rdi,-0x320(%rbp)
 	movabs $0xffffc1ffffffffff,%r13
 	data16 lea 0x4ccb52(%rip),%rdi        
 	data16 data16 rex.W call 149ab0 <__tls_get_addr@plt>
@@ -960186,15 +960186,15 @@
 	lea    -0x280(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    5662c7 <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x1af7>
 	lea    -0x280(%rbp),%rsi
 	call   549c40 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0xd50>
 	jmp    56635b <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x1b8b>
 	mov    0x4d8ab4(%rip),%rax        # a3f830 <c10::detail::getMaybeFakeTypePtr_<c10::optional<at::Tensor>, false>::call()::inner_type@@Base+0x270>
-	cmpb   $0x0,0xfa8(%rax)
+	cmpb   $0x0,0xfc8(%rax)
 	je     56649b <fbgemm_gpu::jagged_index_select_2d(at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x1ccb>
 	sub    $0x8,%rsp
 	mov    %rbx,%r8
 	mov    %r13,%rcx
 	mov    -0x2b0(%rbp),%r9
 	push   $0x0
 	mov    -0x2c0(%rbp),%rdi
@@ -967561,15 +967561,15 @@
 	je     56e320 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x360>
 	cmp    $0x9,%r13w
 	je     56e330 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x370>
 	cmp    $0x6,%r13w
 	je     56e340 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x380>
 	cmp    $0xc,%r13w
 	je     56e350 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x390>
-	add    $0x6c,%edx
+	add    $0x6d,%edx
 	cmp    $0x18,%r13w
 	mov    $0x0,%r13d
 	cmove  %edx,%r13d
 	nopl   0x0(%rax)
 	mov    -0x1c0(%rbp),%rax
 	mov    (%rax),%rdi
 	call   147060 <c10::impl::OperatorEntry::schema() const@plt>
@@ -967695,24 +967695,24 @@
 	call   54ad60 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1e70>
 	mov    %rbx,%rdi
 	call   1493d0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::~vector()@plt>
 	mov    -0x198(%rbp),%rax
 	mov    %rax,(%r14)
 	jmp    56e1da <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x21a>
 	nopl   (%rax)
-	lea    0x2c(%rdx),%r13d
+	lea    0x2d(%rdx),%r13d
 	jmp    56e0a8 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0xe8>
 	nopl   0x0(%rax)
-	lea    0x4c(%rdx),%r13d
+	lea    0x4d(%rdx),%r13d
 	jmp    56e0a8 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0xe8>
 	nopl   0x0(%rax)
-	lea    0x3c(%rdx),%r13d
+	lea    0x3d(%rdx),%r13d
 	jmp    56e0a8 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0xe8>
 	nopl   0x0(%rax)
-	lea    0x5c(%rdx),%r13d
+	lea    0x5d(%rdx),%r13d
 	jmp    56e0a8 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0xe8>
 	nopl   0x0(%rax)
 	mov    0x10(%r15),%rax
 	test   %rax,%rax
 	jne    56e26c <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double)@@Base+0x2ac>
 	sub    $0x8,%rsp
 	lea    -0x198(%rbp),%r13
@@ -968486,15 +968486,15 @@
 	je     56f168 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x258>
 	cmp    $0x9,%r13w
 	je     56f178 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x268>
 	cmp    $0x6,%r13w
 	je     56f240 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x330>
 	cmp    $0xc,%r13w
 	je     56f280 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x370>
-	add    $0x6c,%edx
+	add    $0x6d,%edx
 	cmp    $0x18,%r13w
 	mov    $0x0,%r13d
 	cmove  %edx,%r13d
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rdi
 	call   147060 <c10::impl::OperatorEntry::schema() const@plt>
@@ -968573,18 +968573,18 @@
 	ret
 	mov    -0x1a8(%rbp),%rdi
 	mov    %rax,%rsi
 	mov    %r13d,%edx
 	call   145770 <c10::Dispatcher::runRecordFunction(at::RecordFunction&, std::reference_wrapper<c10::FunctionSchema const>, c10::DispatchKey)@plt>
 	jmp    56f0eb <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x1db>
 	nopl   0x0(%rax)
-	lea    0x2c(%rdx),%r13d
+	lea    0x2d(%rdx),%r13d
 	jmp    56eff0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
-	lea    0x4c(%rdx),%r13d
+	lea    0x4d(%rdx),%r13d
 	jmp    56eff0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
 	test   %rax,%rax
 	je     56f289 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x379>
 	sub    $0x8,%rsp
 	mov    0x18(%rbp),%r9
 	mov    0x10(%rbp),%r8
@@ -968618,29 +968618,29 @@
 	mov    %rbx,%rsi
 	call   54ad60 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1e70>
 	mov    %rbx,%rdi
 	call   1493d0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::~vector()@plt>
 	mov    -0x198(%rbp),%rax
 	mov    %rax,(%r14)
 	jmp    56f132 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x222>
-	lea    0x3c(%rdx),%r13d
+	lea    0x3d(%rdx),%r13d
 	jmp    56eff0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
 	push   0x20(%rbp)
 	mov    0x10(%rbp),%r9
 	mov    %r15,%r8
 	mov    %r12,%rcx
 	mov    -0x1b8(%rbp),%rdx
 	push   0x18(%rbp)
 	mov    %r14,%rdi
 	mov    -0x1b0(%rbp),%rsi
 	call   147e30 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@plt>
 	jmp    56f130 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0x220>
 	nopl   0x0(%rax,%rax,1)
-	lea    0x5c(%rdx),%r13d
+	lea    0x5d(%rdx),%r13d
 	jmp    56eff0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, at::Tensor const&)@@Base+0xe0>
 	push   0x20(%rbp)
 	lea    -0x198(%rbp),%r13
 	mov    %r15,%r8
 	mov    %r12,%rcx
 	mov    0x10(%rbp),%r9
 	push   0x18(%rbp)
@@ -969265,15 +969265,15 @@
 	je     56fe98 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x228>
 	cmp    $0x9,%r13w
 	je     56fea8 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x238>
 	cmp    $0x6,%r13w
 	je     56ff70 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x300>
 	cmp    $0xc,%r13w
 	je     56ffb0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x340>
-	add    $0x6c,%edx
+	add    $0x6d,%edx
 	cmp    $0x18,%r13w
 	mov    $0x0,%r13d
 	cmove  %edx,%r13d
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x1a8(%rbp),%rax
 	mov    (%rax),%rdi
 	call   147060 <c10::impl::OperatorEntry::schema() const@plt>
@@ -969340,18 +969340,18 @@
 	nopl   0x0(%rax,%rax,1)
 	mov    -0x198(%rbp),%rdi
 	mov    %rax,%rsi
 	mov    %r13d,%edx
 	call   145770 <c10::Dispatcher::runRecordFunction(at::RecordFunction&, std::reference_wrapper<c10::FunctionSchema const>, c10::DispatchKey)@plt>
 	jmp    56fe1c <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1ac>
 	nopl   0x0(%rax)
-	lea    0x2c(%rdx),%r13d
+	lea    0x2d(%rdx),%r13d
 	jmp    56fd50 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
-	lea    0x4c(%rdx),%r13d
+	lea    0x4d(%rdx),%r13d
 	jmp    56fd50 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
 	test   %rax,%rax
 	je     56ffb9 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x349>
 	mov    0x18(%rbp),%r9
 	mov    0x10(%rbp),%r8
 	mov    %r15,%rcx
@@ -969382,15 +969382,15 @@
 	call   54ad60 <torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >::apply(std::vector<at::Tensor, std::allocator<at::Tensor> >&&)@@Base+0x1e70>
 	mov    %rbx,%rdi
 	call   1493d0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::~vector()@plt>
 	mov    -0x188(%rbp),%rax
 	mov    %rax,(%r14)
 	jmp    56fe5a <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1ea>
 	nopw   0x0(%rax,%rax,1)
-	lea    0x3c(%rdx),%r13d
+	lea    0x3d(%rdx),%r13d
 	jmp    56fd50 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe0>
 	nopl   0x0(%rax)
 	sub    $0x8,%rsp
 	push   0x18(%rbp)
 	mov    0x10(%rbp),%r9
 	mov    %r15,%r8
 	mov    -0x1a8(%rbp),%rdx
@@ -969398,15 +969398,15 @@
 	mov    %r14,%rdi
 	mov    -0x1a0(%rbp),%rsi
 	call   1472f0 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@plt>
 	pop    %rax
 	pop    %rdx
 	jmp    56fe5a <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x1ea>
 	xchg   %ax,%ax
-	lea    0x5c(%rdx),%r13d
+	lea    0x5d(%rdx),%r13d
 	jmp    56fd50 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0xe0>
 	sub    $0x8,%rsp
 	push   0x18(%rbp)
 	mov    0x10(%rbp),%r9
 	mov    %r15,%r8
 	lea    -0x188(%rbp),%r13
 	mov    -0x1a8(%rbp),%rdx
@@ -970939,15 +970939,15 @@
 	and    $0x7fff,%edx
 	jne    571b2d <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x21d>
 	xor    %eax,%eax
 	cmp    $0x9,%r13w
 	jne    571b5d <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x24d>
 	nopl   0x0(%rax,%rax,1)
 	movzbl %al,%eax
-	lea    0x4c(%rax),%r13d
+	lea    0x4d(%rax),%r13d
 	nopw   0x0(%rax,%rax,1)
 	mov    -0x1b8(%rbp),%rax
 	mov    (%rax),%rdi
 	call   147060 <c10::impl::OperatorEntry::schema() const@plt>
 	cmpb   $0x0,-0xdf(%rbp)
 	mov    %rax,%rsi
 	je     571b88 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x278>
@@ -971031,15 +971031,15 @@
 	cmp    $0x9,%r13w
 	je     5719c0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xb0>
 	cmp    $0x6,%r13w
 	je     571c70 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x360>
 	movzbl %al,%eax
 	cmp    $0xc,%r13w
 	je     571cb0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x3a0>
-	add    $0x6c,%eax
+	add    $0x6d,%eax
 	cmp    $0x18,%r13w
 	mov    $0x0,%r13d
 	cmove  %eax,%r13d
 	jmp    5719d0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xc0>
 	nopw   0x0(%rax,%rax,1)
 	mov    -0x1a8(%rbp),%rdi
 	mov    %r13d,%edx
@@ -971083,33 +971083,33 @@
 	mov    %r15,%rdi
 	call   1493d0 <std::vector<c10::IValue, std::allocator<c10::IValue> >::~vector()@plt>
 	mov    -0x198(%rbp),%rax
 	mov    %rax,(%r14)
 	jmp    571aff <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1ef>
 	nopl   (%rax)
 	movzbl %al,%eax
-	lea    0x2c(%rax),%r13d
+	lea    0x2d(%rax),%r13d
 	jmp    5719d0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xc0>
 	nopl   0x0(%rax)
 	movzbl %al,%eax
-	lea    0x3c(%rax),%r13d
+	lea    0x3d(%rax),%r13d
 	jmp    5719d0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xc0>
 	nopl   0x0(%rax)
 	push   0x20(%rbp)
 	mov    0x10(%rbp),%r9
 	mov    %r12,%rcx
 	mov    %rbx,%rsi
 	mov    -0x1b0(%rbp),%r8
 	push   0x18(%rbp)
 	mov    %r14,%rdi
 	mov    -0x1b8(%rbp),%rdx
 	call   148380 <c10::impl::BoxedKernelWrapper<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), void>::call(c10::BoxedKernel const&, c10::OperatorHandle const&, c10::DispatchKeySet, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@plt>
 	jmp    571afd <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0x1ed>
 	nopl   0x0(%rax,%rax,1)
-	lea    0x5c(%rax),%r13d
+	lea    0x5d(%rax),%r13d
 	jmp    5719d0 <at::Tensor c10::Dispatcher::callWithDispatchKeySlowPath<at::Tensor, at::Tensor const&, at::Tensor const&, at::Tensor const&, long>(c10::TypedOperatorHandle<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)> const&, at::StepCallbacks&, c10::DispatchKeySet, c10::KernelFunction const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long)@@Base+0xc0>
 	push   0x20(%rbp)
 	lea    -0x198(%rbp),%r13
 	mov    %r12,%rcx
 	mov    %rbx,%rsi
 	mov    0x10(%rbp),%r9
 	push   0x18(%rbp)
@@ -1018031,15 +1018031,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	jne    5a575b <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x28fb>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r14,%rdi
 	mov    %si,0x152(%rsp)
 	mov    0x150(%rsp),%eax
 	lea    0x3d2d28(%rip),%rsi        # 9784a6 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1c6>
 	vmovdqu 0x168(%rsp),%xmm6
@@ -1018139,15 +1018139,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a5a40 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x2be0>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r13,%rdx
 	lea    0x3d2a3c(%rip),%rsi        # 97848b <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1ab>
 	mov    %r14,%rdi
 	mov    %cx,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	vmovq  0x48e201(%rip),%xmm4        # a33c68 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<std::vector<at::Tensor, std::allocator<at::Tensor> > >()@@Base+0x4cb558>
 	mov    %r13,%rdi
@@ -1018226,15 +1018226,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a5c8a <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x2e2a>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	lea    0x3cd624(%rip),%rsi        # 9732ba <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x11a>
 	mov    %r14,%rdi
 	mov    %dx,0x152(%rsp)
 	mov    %r13,%rdx
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018307,15 +1018307,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a5eac <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x304c>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3d10a0(%rip),%rsi        # 976f5b <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x13b>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	vmovq  0x49004d(%rip),%xmm6        # a35f20 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<double>()@@Base+0x4ceb90>
 	vmovq  0x49009d(%rip),%xmm7        # a35f78 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<std::vector<long, std::allocator<long> > >()@@Base+0x4cd3a8>
@@ -1018395,15 +1018395,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a60fa <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x329a>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3cd17d(%rip),%rsi        # 973286 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0xe6>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	vmovq  0x48f4e7(%rip),%xmm1        # a35608 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<c10::ArrayRef<c10::SymInt> >()@@Base+0x4bea68>
 	mov    %r13,%rdi
@@ -1018479,15 +1018479,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6330 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x34d0>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3ceae9(%rip),%rsi        # 974e28 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1c88>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018560,15 +1018560,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6552 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x36f2>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3ce89f(%rip),%rsi        # 974e00 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1c60>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018642,15 +1018642,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6778 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x3918>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3ccb9e(%rip),%rsi        # 973325 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x185>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018723,15 +1018723,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6995 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x3b35>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r15d
+	mov    $0x2e,%r15d
 	mov    %r13,%rdx
 	lea    0x3d4863(%rip),%rsi        # 97b208 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x2f28>
 	mov    %r14,%rdi
 	mov    %r15w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018802,15 +1018802,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6bad <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x3d4d>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r11d
+	mov    $0x2e,%r11d
 	mov    %r13,%rdx
 	lea    0x3ce723(%rip),%rsi        # 9752e0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2140>
 	mov    %r14,%rdi
 	mov    %r11w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018881,15 +1018881,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6dc0 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x3f60>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r10d
+	mov    $0x2e,%r10d
 	mov    %r13,%rdx
 	lea    0x3cde98(%rip),%rsi        # 974c68 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1ac8>
 	mov    %r14,%rdi
 	mov    %r10w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1018962,15 +1018962,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a6fdf <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x417f>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r9d
+	mov    $0x2e,%r9d
 	mov    %r13,%rdx
 	lea    0x3cc2ae(%rip),%rsi        # 97329d <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0xfd>
 	mov    %r14,%rdi
 	mov    %r9w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019043,15 +1019043,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a7203 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x43a3>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r8d
+	mov    $0x2e,%r8d
 	mov    %r13,%rdx
 	lea    0x3ce145(%rip),%rsi        # 975358 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x21b8>
 	mov    %r14,%rdi
 	mov    %r8w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019121,15 +1019121,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a7412 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x45b2>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	mov    %r13,%rdx
 	lea    0x3cdf07(%rip),%rsi        # 975328 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2188>
 	mov    %di,0x152(%rsp)
 	mov    %r14,%rdi
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019203,15 +1019203,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a7638 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x47d8>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	mov    %r13,%rdx
 	mov    %r14,%rdi
 	mov    %si,0x152(%rsp)
 	lea    0x3cd64e(%rip),%rsi        # 974ca0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x1b00>
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019283,15 +1019283,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	jne    5a7852 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x49f2>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r12,%rdx
 	lea    0x3cdb5f(%rip),%rsi        # 9753c0 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x2220>
 	mov    %r14,%rdi
 	mov    %cx,0x152(%rsp)
 	mov    0x150(%rsp),%eax
 	xor    %ecx,%ecx
 	vmovdqu 0x168(%rsp),%xmm2
@@ -1019381,15 +1019381,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a7af5 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x4c95>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	lea    0x3cd887(%rip),%rsi        # 975388 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x21e8>
 	mov    %r14,%rdi
 	mov    %dx,0x152(%rsp)
 	mov    %r13,%rdx
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019419,15 +1019419,15 @@
 	call   145f90 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long)>()@plt>
 	mov    0x48a177(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rax,0x1e0(%rsp)
 	jne    5a7be7 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x4d87>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r12,%rdx
 	lea    0x3d088d(%rip),%rsi        # 978483 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1a3>
 	mov    %r14,%rdi
 	mov    %ax,0x1a2(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019452,15 +1019452,15 @@
 	mov    %rax,0x160(%rsp)
 	mov    0x489f70(%rip),%rax        # a31c08 <c10::impl::wrap_kernel_functor_unboxed_<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long), &fbgemm_gpu::stacked_jagged_2d_to_dense_cpu>, std::vector<at::Tensor, std::allocator<at::Tensor> >, c10::guts::typelist::typelist<at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long> >, std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long)>::call(c10::OperatorKernel*, c10::DispatchKeySet, at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long)@@Base+0x26b138>
 	mov    %rax,0x168(%rsp)
 	call   145f90 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::vector<at::Tensor, std::allocator<at::Tensor> > (at::Tensor, at::Tensor, std::vector<long, std::allocator<long> > const&, std::vector<long, std::allocator<long> > const&, long)>()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	jne    5a7cb7 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x4e57>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	mov    0x150(%rsp),%eax
 	lea    0x3d07c4(%rip),%rsi        # 97849e <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1be>
 	vmovdqu 0x168(%rsp),%xmm1
@@ -1019558,15 +1019558,15 @@
 	movq   $0x0,0x178(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x20(%rsp),%rdx
 	cmpb   $0x0,0x100(%rsp)
 	mov    %rdx,0x140(%rsp)
 	jne    5a7f8f <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x512f>
 	movb   $0x1,0x100(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %rbx,%rdx
 	lea    0x3cd6d2(%rip),%rsi        # 975670 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x24d0>
 	mov    %r14,%rdi
 	mov    %ax,0x102(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %rbx,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019641,15 +1019641,15 @@
 	movq   $0x0,0x178(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x60(%rsp),%rdx
 	cmpb   $0x0,0x100(%rsp)
 	mov    %rdx,0x140(%rsp)
 	jne    5a81b9 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5359>
 	movb   $0x1,0x100(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %rbx,%rdx
 	lea    0x3d02f1(%rip),%rsi        # 9784b9 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1d9>
 	mov    %r14,%rdi
 	mov    %ax,0x102(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %rbx,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019724,15 +1019724,15 @@
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x60(%rsp),%rdx
 	cmpb   $0x0,0x150(%rsp)
 	mov    %rdx,0x190(%rsp)
 	jne    5a83e5 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5585>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x3d00e1(%rip),%rsi        # 9784d5 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x1f5>
 	mov    %r14,%rdi
 	mov    %ax,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019806,15 +1019806,15 @@
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x60(%rsp),%rdx
 	cmpb   $0x0,0x150(%rsp)
 	mov    %rdx,0x190(%rsp)
 	jne    5a8608 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x57a8>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r11d
+	mov    $0x2e,%r11d
 	mov    %r13,%rdx
 	lea    0x3cfdfb(%rip),%rsi        # 978413 <typeinfo name for std::_Sp_counted_ptr<c10::ListType*, (__gnu_cxx::_Lock_policy)2>@@Base+0x133>
 	mov    %r14,%rdi
 	mov    %r11w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019889,15 +1019889,15 @@
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x60(%rsp),%rdx
 	cmpb   $0x0,0x150(%rsp)
 	mov    %rdx,0x190(%rsp)
 	jne    5a8831 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x59d1>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r10d
+	mov    $0x2e,%r10d
 	mov    %r13,%rdx
 	lea    0x3caa89(%rip),%rsi        # 9732ca <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x12a>
 	mov    %r14,%rdi
 	mov    %r10w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1019973,15 +1019973,15 @@
 	movq   $0x0,0x1c8(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	mov    0x60(%rsp),%rdx
 	cmpb   $0x0,0x150(%rsp)
 	mov    %rdx,0x190(%rsp)
 	jne    5a8a63 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5c03>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%r9d
+	mov    $0x2e,%r9d
 	mov    %r13,%rdx
 	lea    0x3ce519(%rip),%rsi        # 976f8c <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x16c>
 	mov    %r14,%rdi
 	mov    %r9w,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1020009,15 +1020009,15 @@
 	call   14b690 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)>()@plt>
 	mov    0x489212(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rax,0x1e0(%rsp)
 	jne    5a8b4c <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5cec>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%r8d
+	mov    $0x2e,%r8d
 	mov    %r12,%rdx
 	lea    0x3ce461(%rip),%rsi        # 976fbd <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x19d>
 	mov    %r14,%rdi
 	mov    %r8w,0x1a2(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1020042,15 +1020042,15 @@
 	mov    %rax,0x168(%rsp)
 	mov    0x48c18a(%rip),%rax        
 	mov    %rax,0x180(%rsp)
 	call   14b690 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	jne    5a8c1d <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5dbd>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	xor    %ecx,%ecx
 	lea    0x3ca6ae(%rip),%rsi        # 9732d9 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x139>
 	mov    %r12,%rdx
 	mov    %di,0x152(%rsp)
 	mov    0x150(%rsp),%eax
 	mov    %r14,%rdi
 	vmovdqu 0x168(%rsp),%xmm5
@@ -1020099,15 +1020099,15 @@
 	call   14b690 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)>()@plt>
 	mov    0x488fbb(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rax,0x1e0(%rsp)
 	jne    5a8da3 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x5f43>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	mov    %r12,%rdx
 	mov    %r14,%rdi
 	mov    %si,0x1a2(%rsp)
 	lea    0x3ce1e6(%rip),%rsi        # 976fa3 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x183>
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	vmovdqa 0xc0(%rsp),%xmm7
 	mov    %r12,%rdi
@@ -1020182,15 +1020182,15 @@
 	movzwl 0x1e2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x150(%rsp)
 	mov    %r15,0x190(%rsp)
 	jne    5a8fcb <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x616b>
 	movb   $0x1,0x150(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r13,%rdx
 	lea    0x3ca311(%rip),%rsi        # 9732eb <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x14b>
 	mov    %r14,%rdi
 	mov    %cx,0x152(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1020218,15 +1020218,15 @@
 	call   14b690 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, long)>()@plt>
 	mov    0x488cac(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rax,0x1e0(%rsp)
 	jne    5a90b2 <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x6252>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	lea    0x3cdeb5(%rip),%rsi        # 976f73 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<std::tuple<at::Tensor, at::Tensor> (at::Tensor const&, at::Tensor const&, at::Tensor const&, long), &fbgemm_gpu::jagged_slice>, std::tuple<at::Tensor, at::Tensor>, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, long> >@@Base+0x153>
 	mov    %r14,%rdi
 	mov    %dx,0x1a2(%rsp)
 	mov    %r12,%rdx
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	vmovq  0x48a50f(%rip),%xmm4        # a335e8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<bool>()@@Base+0x26ff68>
 	vmovdqa 0x50(%rsp),%xmm1
@@ -1020307,15 +1020307,15 @@
 	movzwl 0x192(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x100(%rsp)
 	mov    %r12,0x140(%rsp)
 	jne    5a930e <fbgemm_gpu::jagged_index_add_2d_forward_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long)@@Base+0x64ae>
 	movb   $0x1,0x100(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %rbx,%rdx
 	lea    0x3ca0bf(%rip),%rsi        # 9733dc <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PermutePooledEmbsFunctionSplit<&fbgemm_gpu::permute_pooled_embs_split_cpu> >*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x23c>
 	mov    %r14,%rdi
 	mov    %ax,0x102(%rsp)
 	call   581d90 <c10::impl::make_boxed_from_unboxed_functor<c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double), &fbgemm_gpu::jagged_to_padded_dense_forward_meta>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, c10::ArrayRef<c10::SymInt> const&, double> >, false>::call(c10::OperatorKernel*, c10::OperatorHandle const&, c10::DispatchKeySet, std::vector<c10::IValue, std::allocator<c10::IValue> >*)@@Base+0x88e0>
 	mov    %rbx,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1536217,15 +1536217,15 @@
 	mov    %rax,0x28(%rsp)
 	mov    0x252fd0(%rip),%rax        # a33f60 <typeinfo for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)@@Base+0x7b58>
 	mov    %rax,0x40(%rsp)
 	call   147bf0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&)>()@plt>
 	cmpb   $0x0,0x10(%rsp)
 	jne    7e0fa6 <fbgemm_gpu::padding_fused_tbe_input_combine_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x18a6>
 	movb   $0x1,0x10(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	vmovdqu 0x28(%rsp),%xmm1
 	xor    %ecx,%ecx
 	mov    %rbp,%rdx
 	mov    %si,0x12(%rsp)
 	mov    0x10(%rsp),%eax
 	mov    %r12,%rdi
 	lea    0x19b150(%rip),%rsi        # 97c119 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool), &fbgemm_gpu::jagged_slice_forward_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool> >@@Base+0x199>
@@ -1536270,15 +1536270,15 @@
 	mov    %rax,0x28(%rsp)
 	mov    0x254229(%rip),%rax        # a352d8 <typeinfo for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&)@@Base+0x8ea8>
 	mov    %rax,0x40(%rsp)
 	call   14af10 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&)>()@plt>
 	cmpb   $0x0,0x10(%rsp)
 	jne    7e10c5 <fbgemm_gpu::padding_fused_tbe_input_combine_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x19c5>
 	movb   $0x1,0x10(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	vmovdqu 0x28(%rsp),%xmm3
 	mov    %rbp,%rdx
 	mov    %r12,%rdi
 	mov    %cx,0x12(%rsp)
 	mov    0x10(%rsp),%eax
 	xor    %ecx,%ecx
 	lea    0x19b043(%rip),%rsi        # 97c12b <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool), &fbgemm_gpu::jagged_slice_forward_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool> >@@Base+0x1ab>
@@ -1536323,15 +1536323,15 @@
 	mov    %rax,0x28(%rsp)
 	mov    0x2505c2(%rip),%rax        # a31790 <typeinfo for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x5338>
 	mov    %rax,0x40(%rsp)
 	call   1471e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0x10(%rsp)
 	jne    7e11e4 <fbgemm_gpu::padding_fused_tbe_input_combine_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x1ae4>
 	movb   $0x1,0x10(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	vmovdqu 0x28(%rsp),%xmm5
 	xor    %ecx,%ecx
 	mov    %r12,%rdi
 	mov    %dx,0x12(%rsp)
 	mov    0x10(%rsp),%eax
 	mov    %rbp,%rdx
 	lea    0x19bb29(%rip),%rsi        # 97cd30 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool), &fbgemm_gpu::jagged_slice_forward_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool> >@@Base+0xdb0>
@@ -1536376,15 +1536376,15 @@
 	mov    %rax,0x28(%rsp)
 	mov    0x252b73(%rip),%rax        # a33e60 <typeinfo for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, long)@@Base+0x79e0>
 	mov    %rax,0x40(%rsp)
 	call   147b50 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, long)>()@plt>
 	cmpb   $0x0,0x10(%rsp)
 	jne    7e1303 <fbgemm_gpu::padding_fused_tbe_input_combine_cpu(std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, at::Tensor const&, long)@@Base+0x1c03>
 	movb   $0x1,0x10(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x28(%rsp),%xmm7
 	xor    %ecx,%ecx
 	mov    %rbp,%rdx
 	mov    %ax,0x12(%rsp)
 	mov    0x10(%rsp),%eax
 	lea    0x19ba2d(%rip),%rsi        # 97cd50 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool), &fbgemm_gpu::jagged_slice_forward_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&, long, long, bool> >@@Base+0xdd0>
 	mov    %r12,%rdi
@@ -1540869,15 +1540869,15 @@
 	mov    %rax,0x18(%rsp)
 	mov    0x24de96(%rip),%rax        # a342b8 <typeinfo for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x7d70>
 	mov    %rax,0x30(%rsp)
 	call   146220 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)>()@plt>
 	cmpb   $0x0,(%rsp)
 	jne    7e6436 <fbgemm_gpu::recat_embedding_grad_output_mixed_D_cpu(at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x2df6>
 	movb   $0x1,(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x18(%rsp),%xmm1
 	xor    %ecx,%ecx
 	mov    %rbp,%rdi
 	mov    %ax,0x2(%rsp)
 	mov    (%rsp),%eax
 	lea    0x50(%rsp),%r12
 	lea    0x19708e(%rip),%rsi        # 97d4e8 <typeinfo name for std::tuple<at::Tensor, at::Tensor, at::Tensor> (std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, std::vector<at::Tensor, std::allocator<at::Tensor> > const&, long)@@Base+0x228>
@@ -1545091,15 +1545091,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247754(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eaa5b <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x3bb>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	mov    0x2472d9(%rip),%rbx        
 	vmovdqu 0xb8(%rsp),%xmm4
 	lea    0xf0(%rsp),%r12
 	mov    %di,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
@@ -1545147,15 +1545147,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24afd6(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   147e80 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, bool)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eabd9 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x539>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %si,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192c96(%rip),%rsi        # 97d892 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x192>
 	vmovdqu 0xb8(%rsp),%xmm6
@@ -1545200,15 +1545200,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24746f(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ead40 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x6a0>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r12,%rdx
 	lea    0x1934e1(%rip),%rsi        # 97e230 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xb30>
 	mov    %r13,%rdi
 	mov    %cx,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	xor    %ecx,%ecx
 	vmovdqu 0xb8(%rsp),%xmm4
@@ -1545253,15 +1545253,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247308(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eaea7 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x807>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	xor    %ecx,%ecx
 	lea    0x19339b(%rip),%rsi        # 97e250 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xb50>
 	mov    %r13,%rdi
 	mov    %dx,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	mov    %r12,%rdx
 	vmovdqu 0xb8(%rsp),%xmm6
@@ -1545306,15 +1545306,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247b79(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   147080 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor& (at::Tensor&, at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb00e <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x96e>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x193247(%rip),%rsi        # 97e278 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xb78>
 	vmovdqu 0xb8(%rsp),%xmm2
@@ -1545359,15 +1545359,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24703a(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb175 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0xad5>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x193108(%rip),%rsi        # 97e2a0 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xba0>
 	vmovdqu 0xb8(%rsp),%xmm4
@@ -1545412,15 +1545412,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24a8d3(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   147e80 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, bool)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb2dc <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0xc3c>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x1925ae(%rip),%rsi        # 97d8ad <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x1ad>
 	vmovdqu 0xb8(%rsp),%xmm6
@@ -1545465,15 +1545465,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x246d6c(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb443 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0xda3>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192e62(%rip),%rsi        # 97e2c8 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xbc8>
 	vmovdqu 0xb8(%rsp),%xmm1
@@ -1545518,15 +1545518,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24876d(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb5aa <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0xf0a>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192d1b(%rip),%rsi        # 97e2e8 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xbe8>
 	vmovdqu 0xb8(%rsp),%xmm3
@@ -1545571,15 +1545571,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247476(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   147080 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor& (at::Tensor&, at::Tensor const&)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb711 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x1071>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%r11d
+	mov    $0x2e,%r11d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %r11w,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192bda(%rip),%rsi        # 97e310 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xc10>
 	vmovdqu 0xb8(%rsp),%xmm5
@@ -1545624,15 +1545624,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x24849d(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb87a <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x11da>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%r10d
+	mov    $0x2e,%r10d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %r10w,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192a99(%rip),%rsi        # 97e338 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xc38>
 	vmovdqu 0xb8(%rsp),%xmm7
@@ -1545677,15 +1545677,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x248334(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7eb9e3 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x1343>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%r9d
+	mov    $0x2e,%r9d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %r9w,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192958(%rip),%rsi        # 97e360 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xc60>
 	vmovdqu 0xb8(%rsp),%xmm2
@@ -1545730,15 +1545730,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x2481cb(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ebb4c <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x14ac>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%r8d
+	mov    $0x2e,%r8d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %r8w,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x192817(%rip),%rsi        # 97e388 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xc88>
 	vmovdqu 0xb8(%rsp),%xmm4
@@ -1545783,15 +1545783,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x248062(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ebcb5 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x1615>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	xor    %ecx,%ecx
 	lea    0x1926f5(%rip),%rsi        # 97e3b8 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xcb8>
 	mov    %r12,%rdx
 	mov    %di,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	mov    %r13,%rdi
 	vmovdqu 0xb8(%rsp),%xmm6
@@ -1545836,15 +1545836,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247efb(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145f70 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ebe1c <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x177c>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %si,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x1925a1(%rip),%rsi        # 97e3e0 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xce0>
 	vmovdqu 0xb8(%rsp),%xmm1
@@ -1545889,15 +1545889,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247bb4(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145ac0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ebf83 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x18e3>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r12,%rdx
 	lea    0x192476(%rip),%rsi        # 97e408 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0xd08>
 	mov    %r13,%rdi
 	mov    %cx,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	xor    %ecx,%ecx
 	vmovdqu 0xb8(%rsp),%xmm3
@@ -1545999,15 +1545999,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x132(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ec26b <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x1bcb>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	xor    %ecx,%ecx
 	lea    0x19164f(%rip),%rsi        # 97d8c8 <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x1c8>
 	mov    %r13,%rdi
 	mov    %dx,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	mov    %r12,%rdx
 	vmovdqu 0xb8(%rsp),%xmm1
@@ -1546052,15 +1546052,15 @@
 	mov    %rax,0xb8(%rsp)
 	mov    0x247765(%rip),%rax        
 	mov    %rax,0xd0(%rsp)
 	call   145ac0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@plt>
 	cmpb   $0x0,0xa0(%rsp)
 	jne    7ec3d2 <fbgemm_gpu::float_or_half_to_fusednbitrowwise_cpu(at::Tensor const&, long)@@Base+0x1d32>
 	movb   $0x1,0xa0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0xa2(%rsp)
 	mov    0xa0(%rsp),%eax
 	lea    0x1914e8(%rip),%rsi        # 97d8dd <typeinfo name for at::Tensor (at::Tensor const&, std::vector<long, std::allocator<long> > const&)@@Base+0x1dd>
 	vmovdqu 0xb8(%rsp),%xmm3
@@ -1661954,15 +1661954,15 @@
 	call   1497e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, c10::optional<at::Tensor> > (at::Tensor const&, at::Tensor const&, at::Tensor const&, c10::optional<at::Tensor> const&, c10::optional<long> const&)>()@plt>
 	mov    0x1c4608(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86d756 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x2f56>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	lea    0x260(%rsp),%r12
 	lea    0x1122ce(%rip),%rsi        # 97fa38 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x418>
 	mov    %r15,%rdi
 	mov    %dx,0x262(%rsp)
 	mov    %r12,%rdx
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r12,%rdi
@@ -1661988,15 +1661988,15 @@
 	call   1497e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, c10::optional<at::Tensor> > (at::Tensor const&, at::Tensor const&, at::Tensor const&, c10::optional<at::Tensor> const&, c10::optional<long> const&)>()@plt>
 	mov    0x1c452e(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86d830 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3030>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r12,%rdx
 	lea    0x11220d(%rip),%rsi        # 97fa4c <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x42c>
 	mov    %r15,%rdi
 	mov    %ax,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1662023,15 +1662023,15 @@
 	call   1497e0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<std::tuple<at::Tensor, at::Tensor, c10::optional<at::Tensor> > (at::Tensor const&, at::Tensor const&, at::Tensor const&, c10::optional<at::Tensor> const&, c10::optional<long> const&)>()@plt>
 	mov    0x1c444e(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86d910 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3110>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r12,%rdx
 	lea    0x112144(%rip),%rsi        # 97fa63 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x443>
 	mov    %r15,%rdi
 	mov    %ax,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1662059,15 +1662059,15 @@
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	mov    0x1c4367(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86d9f7 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x31f7>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r12,%rdx
 	lea    0x112074(%rip),%rsi        # 97fa7a <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x45a>
 	mov    %r15,%rdi
 	mov    %ax,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovq  0x1c5982(%rip),%xmm6        # a333a0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<at::Tensor>()@@Base+0x517d70>
 	vmovq  0x1c7baa(%rip),%xmm5        # a355d0 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<long>()@@Base+0x51aa80>
@@ -1662153,15 +1662153,15 @@
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    86dc78 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3478>
 	movb   $0x1,0x200(%rsp)
 	lea    0x200(%rsp),%r13
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	lea    0x111dfd(%rip),%rsi        # 97fa89 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x469>
 	mov    %r15,%rdi
 	mov    %r13,%rdx
 	mov    %ax,0x202(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovq  0x1c3be1(%rip),%xmm7        # a31888 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<c10::optional<at::Tensor> >()@@Base+0x5110b8>
 	vmovq  0x1c5939(%rip),%xmm6        # a335e8 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<bool>()@@Base+0x26ff68>
@@ -1662256,15 +1662256,15 @@
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x140(%rsp)
 	mov    %rbx,0x180(%rsp)
 	jne    86df3a <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x373a>
 	movb   $0x1,0x140(%rsp)
 	mov    0x138(%rsp),%rbx
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	lea    0x114d4a(%rip),%rsi        # 982c98 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x3678>
 	mov    %r15,%rdi
 	mov    %ax,0x142(%rsp)
 	mov    %rbx,%rdx
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovdqa 0x40(%rsp),%xmm7
 	mov    %rbx,%rdi
@@ -1662344,15 +1662344,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	jne    86e18d <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x398d>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%ebx
+	mov    $0x2e,%ebx
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %bx,0x1a2(%rsp)
 	mov    0x1a0(%rsp),%eax
 	lea    0x1118f4(%rip),%rsi        # 97faa4 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x484>
 	vmovdqu 0x1b8(%rsp),%xmm6
@@ -1662401,15 +1662401,15 @@
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	mov    0x1c3a4b(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86e313 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3b13>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%r11d
+	mov    $0x2e,%r11d
 	mov    %r12,%rdx
 	lea    0x11179b(%rip),%rsi        # 97fabe <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x49e>
 	mov    %r15,%rdi
 	mov    %r11w,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1662436,15 +1662436,15 @@
 	lea    0x238(%rsp),%rax
 	mov    %rax,%rdi
 	mov    %rax,0x130(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    86e3f4 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3bf4>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%r10d
+	mov    $0x2e,%r10d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %r10w,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x1116c3(%rip),%rsi        # 97fadc <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x4bc>
 	vmovdqu 0x218(%rsp),%xmm4
@@ -1662493,15 +1662493,15 @@
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	mov    0x1c37e2(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    86e57c <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3d7c>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%r9d
+	mov    $0x2e,%r9d
 	mov    %r12,%rdx
 	lea    0x11156e(%rip),%rsi        # 97fafa <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x4da>
 	mov    %r15,%rdi
 	mov    %r9w,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovdqa 0xb0(%rsp),%xmm1
 	mov    %r12,%rdi
@@ -1662576,15 +1662576,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    86e7ad <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x3fad>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%r8d
+	mov    $0x2e,%r8d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %r8w,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x111345(%rip),%rsi        # 97fb17 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x4f7>
 	vmovdqu 0x218(%rsp),%xmm2
@@ -1662682,15 +1662682,15 @@
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rbx,0x1e0(%rsp)
 	jne    86ea8f <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x428f>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	mov    %r14,%rdx
 	lea    0x111094(%rip),%rsi        # 97fb32 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x512>
 	mov    %di,0x1a2(%rsp)
 	mov    %r15,%rdi
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r14,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1662760,15 +1662760,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    86ec97 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x4497>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	mov    %r13,%rdx
 	mov    %r15,%rdi
 	mov    %si,0x202(%rsp)
 	lea    0x110e9c(%rip),%rsi        # 97fb4d <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x52d>
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1662838,15 +1662838,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    86eea0 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x46a0>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r12,%rdx
 	lea    0x110cac(%rip),%rsi        # 97fb5b <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x53b>
 	mov    %r15,%rdi
 	mov    %cx,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	xor    %ecx,%ecx
 	vmovdqu 0x218(%rsp),%xmm2
@@ -1662953,15 +1662953,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	jne    86f1ba <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x49ba>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	xor    %ecx,%ecx
 	lea    0x1109ac(%rip),%rsi        # 97fb74 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x554>
 	mov    %r15,%rdi
 	mov    %dx,0x1a2(%rsp)
 	mov    0x1a0(%rsp),%eax
 	mov    %r12,%rdx
 	vmovdqu 0x1b8(%rsp),%xmm3
@@ -1663058,15 +1663058,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	jne    86f495 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x4c95>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0x1a2(%rsp)
 	mov    0x1a0(%rsp),%eax
 	lea    0x113808(%rip),%rsi        # 982cc0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x36a0>
 	vmovdqu 0x1b8(%rsp),%xmm7
@@ -1663162,15 +1663162,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	jne    86f767 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x4f67>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0x1a2(%rsp)
 	mov    0x1a0(%rsp),%eax
 	lea    0x11352e(%rip),%rsi        # 982cb8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x3698>
 	vmovdqu 0x1b8(%rsp),%xmm6
@@ -1663268,15 +1663268,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    86fa44 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5244>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x11012b(%rip),%rsi        # 97fb92 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x572>
 	vmovdqu 0x218(%rsp),%xmm1
@@ -1663379,15 +1663379,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	jne    86fd43 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5543>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0x1a2(%rsp)
 	mov    0x1a0(%rsp),%eax
 	lea    0x10fa63(%rip),%rsi        # 97f7c9 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x1a9>
 	vmovdqu 0x1b8(%rsp),%xmm4
@@ -1663484,15 +1663484,15 @@
 	mov    %cx,0x42(%rax)
 	movq   $0x0,0x288(%rsp)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    870017 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5817>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	mov    %r13,%rdx
 	lea    0x10fb7c(%rip),%rsi        # 97fba2 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x582>
 	mov    %r15,%rdi
 	mov    %ax,0x202(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1663566,15 +1663566,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    87023d <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5a3d>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%ebx
+	mov    $0x2e,%ebx
 	mov    %r13,%rdx
 	lea    0x10f64b(%rip),%rsi        # 97f897 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x277>
 	mov    %r15,%rdi
 	mov    %bx,0x202(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovdqa 0x120(%rsp),%xmm6
 	mov    %r13,%rdi
@@ -1663653,15 +1663653,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    87048c <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5c8c>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%r11d
+	mov    $0x2e,%r11d
 	mov    %r13,%rdx
 	lea    0x10f714(%rip),%rsi        # 97fbb0 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x590>
 	mov    %r15,%rdi
 	mov    %r11w,0x202(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1663686,15 +1663686,15 @@
 	mov    %rax,0x218(%rsp)
 	mov    0x1c1c4d(%rip),%rax        
 	mov    %rax,0x230(%rsp)
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    870562 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5d62>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%r10d
+	mov    $0x2e,%r10d
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %r10w,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x10f641(%rip),%rsi        # 97fbc8 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x5a8>
 	vmovdqu 0x218(%rsp),%xmm4
@@ -1663743,15 +1663743,15 @@
 	call   145e30 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&)>()@plt>
 	mov    0x1c1674(%rip),%rax        
 	add    $0x18,%rax
 	cmpb   $0x0,0x260(%rsp)
 	mov    %rax,0x2a0(%rsp)
 	jne    8706ea <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x5eea>
 	movb   $0x1,0x260(%rsp)
-	mov    $0x2d,%r9d
+	mov    $0x2e,%r9d
 	mov    %r12,%rdx
 	lea    0x10f4e7(%rip),%rsi        # 97fbe1 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x5c1>
 	mov    %r15,%rdi
 	mov    %r9w,0x262(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r12,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1663825,15 +1663825,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    870912 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x6112>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%r8d
+	mov    $0x2e,%r8d
 	mov    %r13,%rdx
 	lea    0x10f2d8(%rip),%rsi        # 97fbfa <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x5da>
 	mov    %r15,%rdi
 	mov    %r8w,0x202(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1663906,15 +1663906,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    870b31 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x6331>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%edi
+	mov    $0x2e,%edi
 	mov    %r13,%rdx
 	lea    0x10f0d8(%rip),%rsi        # 97fc18 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x5f8>
 	mov    %di,0x202(%rsp)
 	mov    %r15,%rdi
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1663987,15 +1663987,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    870d4f <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x654f>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%esi
+	mov    $0x2e,%esi
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %si,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x10eec2(%rip),%rsi        # 97fc34 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x614>
 	vmovdqu 0x218(%rsp),%xmm2
@@ -1664096,15 +1664096,15 @@
 	movzwl 0x242(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x1a0(%rsp)
 	mov    %rbx,0x1e0(%rsp)
 	jne    871046 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x6846>
 	movb   $0x1,0x1a0(%rsp)
-	mov    $0x2d,%ecx
+	mov    $0x2e,%ecx
 	mov    %r14,%rdx
 	lea    0x10e99d(%rip),%rsi        # 97f9f2 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x3d2>
 	mov    %r15,%rdi
 	mov    %cx,0x1a2(%rsp)
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	vmovq  0x1c2bfb(%rip),%xmm5        # a33c68 <c10::Type::SingletonOrSharedTypePtr<c10::Type> c10::getTypePtrCopy<std::vector<at::Tensor, std::allocator<at::Tensor> > >()@@Base+0x4cb558>
 	mov    %r14,%rdi
@@ -1664179,15 +1664179,15 @@
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	mov    %rbx,0x240(%rsp)
 	jne    871277 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x6a77>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%edx
+	mov    $0x2e,%edx
 	lea    0x10e769(%rip),%rsi        # 97f9ec <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x3cc>
 	mov    %r15,%rdi
 	mov    %dx,0x202(%rsp)
 	mov    %r13,%rdx
 	call   7f1ea0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor const&, long, long)>()@@Base+0x5e0>
 	mov    %r13,%rdi
 	call   149370 <torch::CppFunction::~CppFunction()@plt>
@@ -1664259,15 +1664259,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x2a2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x200(%rsp)
 	jne    871491 <fbgemm_gpu::pack_segments_forward_cpu(at::Tensor const&, at::Tensor const&, long)@@Base+0x6c91>
 	movb   $0x1,0x200(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r15,%rdi
 	mov    %ax,0x202(%rsp)
 	mov    0x200(%rsp),%eax
 	lea    0x10e78e(%rip),%rsi        # 97fc42 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, long, long), &fbgemm_gpu::_hfp8_to_float_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, long, long> >@@Base+0x622>
 	vmovdqu 0x218(%rsp),%xmm4
@@ -1703858,15 +1703858,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0xd2(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    89a1cc <fbgemm_gpu::pruned_array_lookup_from_row_idx_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0x95c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm6
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xeb079(%rip),%rsi        # 985265 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PackSegmentsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0x485>
 	mov    %r13,%rdi
@@ -1703986,15 +1703986,15 @@
 	mov    %dx,0x40(%rax)
 	movzwl 0x112(%rsp),%edx
 	mov    %dx,0x42(%rax)
 	call   14b0d0 <c10::FunctionSchema::~FunctionSchema()@plt>
 	cmpb   $0x0,0x80(%rsp)
 	jne    89a4b6 <fbgemm_gpu::pruned_array_lookup_from_row_idx_cpu(at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&)@@Base+0xc46>
 	movb   $0x1,0x80(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	xor    %ecx,%ecx
 	mov    %r12,%rdx
 	mov    %r13,%rdi
 	mov    %ax,0x82(%rsp)
 	mov    0x80(%rsp),%eax
 	lea    0xeb40f(%rip),%rsi        # 9858e8 <typeinfo name for std::_Sp_counted_deleter<torch::autograd::CppNode<fbgemm_gpu::PackSegmentsFunction>*, void (*)(torch::autograd::Node*), std::allocator<void>, (__gnu_cxx::_Lock_policy)2>@@Base+0xb08>
 	vmovdqu 0x98(%rsp),%xmm4
@@ -1740099,15 +1740099,15 @@
 	mov    0x171d93(%rip),%rax        # a35210 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, long)@@Base+0x7ce8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   1452f0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8c349c <split_embedding_backward_codegen_dense_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, long, at::Tensor, at::Tensor, long, at::Tensor, double)@@Base+0x641c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xc35a1(%rip),%rsi        # 986a60 <typeinfo name for c10::impl::detail::WrapFunctionIntoFunctor_<c10::CompileTimeFunctionPointer<at::Tensor (at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&), &fbgemm_gpu::pruned_array_lookup_from_row_idx_cpu>, at::Tensor, c10::guts::typelist::typelist<at::Tensor const&, at::Tensor const&, at::Tensor const&, at::Tensor const&> >@@Base+0xfa0>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1747010,15 +1747010,15 @@
 	mov    0x16a17b(%rip),%rax        # a359f8 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, double, long)@@Base+0x83e8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   1474f0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, double, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8cb89c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, long)>()@@Base+0x2c0c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xbb929(%rip),%rsi        # 9871e8 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, long)@@Base+0x2e8>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1754173,15 +1754173,15 @@
 	mov    0x16004b(%rip),%rax        # a341e8 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)@@Base+0x6af0>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   149fc0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8d41bc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, double, long)>()@@Base+0x2d9c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xb39b1(%rip),%rsi        # 987b90 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, double, long)@@Base+0x4d0>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1762505,15 +1762505,15 @@
 	mov    0x156283(%rip),%rax        # a34640 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)@@Base+0x6e60>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14bb00 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8de3dc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)>()@@Base+0x2c0c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xaa009(%rip),%rsi        # 988408 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)@@Base+0x2c8>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1769500,15 +1769500,15 @@
 	mov    0x14c7d3(%rip),%rax        # a331b0 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)@@Base+0x58e8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   1467a0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8e69fc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)>()@@Base+0x2c0c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0xa20f1(%rip),%rsi        # 988b10 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)@@Base+0x210>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1773813,15 +1773813,15 @@
 	mov    0x146273(%rip),%rax        # a32130 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x4818>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14abd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8ebedc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)>()@@Base+0xb3c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x9d1c9(%rip),%rsi        # 9890c8 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)@@Base+0x148>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1775151,15 +1775151,15 @@
 	mov    0x1447d3(%rip),%rax        # a32130 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x4818>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14abd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8ed97c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@@Base+0xb3c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x9bd41(%rip),%rsi        # 9896e0 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x160>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1776437,15 +1776437,15 @@
 	mov    0x142e13(%rip),%rax        # a32130 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x4818>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14abd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8ef33c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@@Base+0x24fc>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x9a951(%rip),%rsi        # 989cb0 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x730>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1777723,15 +1777723,15 @@
 	mov    0x141453(%rip),%rax        # a32130 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x4818>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14abd0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f0cfc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@@Base+0x3ebc>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x99581(%rip),%rsi        # 98a2a0 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0xd20>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1778973,15 +1778973,15 @@
 	mov    0x141843(%rip),%rax        # a33e20 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)@@Base+0x63f8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   1480f0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f25fc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)>()@@Base+0x57bc>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x98271(%rip),%rsi        # 98a890 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, double, long, long)@@Base+0x1310>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1780194,15 +1780194,15 @@
 	mov    0x140903(%rip),%rax        # a34640 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)@@Base+0x6e60>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14bb00 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f3d5c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)>()@@Base+0xa7c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x970d1(%rip),%rsi        # 98ae50 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)@@Base+0x190>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1781364,15 +1781364,15 @@
 	mov    0x13f283(%rip),%rax        # a34640 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)@@Base+0x6e60>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14bb00 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f53dc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)>()@@Base+0x20fc>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x96019(%rip),%rsi        # 98b418 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)@@Base+0x758>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1782518,15 +1782518,15 @@
 	mov    0x13eac3(%rip),%rax        # a354a0 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0x79a8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   146740 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f69fc <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)>()@@Base+0x371c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x94f91(%rip),%rsi        # 98b9b0 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, double, long)@@Base+0xcf0>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1783602,15 +1783602,15 @@
 	mov    0x13b3e3(%rip),%rax        # a331b0 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)@@Base+0x58e8>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   1467a0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, double, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f7dec <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)>()@@Base+0xa1c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x940a9(%rip),%rsi        # 98beb8 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0x158>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1784653,15 +1784653,15 @@
 	mov    0x13b4e3(%rip),%rax        # a34640 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)@@Base+0x6e60>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   14bb00 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8f917c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)>()@@Base+0x1dac>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x931b9(%rip),%rsi        # 98c358 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0x5f8>
 	vmovdqu %xmm1,0xa8(%rsp)
@@ -1785882,15 +1785882,15 @@
 	mov    0x1398bb(%rip),%rax        # a341e8 <typeinfo for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)@@Base+0x6af0>
 	movq   $0x0,0x60(%rsp)
 	mov    %rax,0x70(%rsp)
 	call   149fc0 <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, double, double, double, long, long, long, double, long, long, long, double, double, long, long)>()@plt>
 	cmpb   $0x0,0x40(%rsp)
 	jne    8fa94c <std::unique_ptr<c10::FunctionSchema, std::default_delete<c10::FunctionSchema> > c10::detail::inferFunctionSchemaFromFunctor<at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)>()@@Base+0x357c>
 	movb   $0x1,0x40(%rsp)
-	mov    $0x2d,%eax
+	mov    $0x2e,%eax
 	vmovdqu 0x58(%rsp),%xmm1
 	vmovdqu 0x68(%rsp),%xmm2
 	xor    %ecx,%ecx
 	mov    %ax,0x42(%rsp)
 	mov    0x40(%rsp),%eax
 	lea    0x91f71(%rip),%rsi        # 98c8e0 <typeinfo name for at::Tensor (at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, long, at::Tensor, long, at::Tensor, at::Tensor, long, c10::optional<at::Tensor>, c10::optional<at::Tensor>, bool, double, bool, long, long, long)@@Base+0xb80>
 	vmovdqu %xmm1,0xa8(%rsp)
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2023.6.21
+Version: 2023.6.22
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 fbgemm_gpu/__init__.py,sha256=hyPNE6QvlwUNM4PlyfKee7j7agkOF2SNoT3EQXJ-pe0,567
 fbgemm_gpu/_fbgemm_gpu_docs.py,sha256=ks59ZF1sbng7P2uhG_taag5310ml9N_y4jU0EDsUhXs,14920
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=rc49BZwtZuu8qsO5MENAlHeswgPUn35aM8Cgr3XtBE0,2747
 fbgemm_gpu/enums.py,sha256=Tg1pBJrcfSIWmWec2WCZkRuMwmCnepKrcACi3ZijZmk,818
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=ONxVPNTiXmbrGwHoFgyHXzktgg7exJJo5o0UDEtUpbg,10709064
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=7vTjk2juwniLOc5fztk8XRsyd9-J6mRqmlBtl4Sepwg,10709064
 fbgemm_gpu/metrics.py,sha256=e5VnTatZjFqcgOfipH7Eqk5lsAkuxY2qsbil3Csy_yk,5648
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=n80gTkNwSA9k0dvJeZhVjzXC08c74o0G-u4MnKs7rek,2339
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=9MWBghoy5eajS4yleFWAMdi0LWV0nNbcIgCkqdkRP5g,2477
 fbgemm_gpu/quantize_comm.py,sha256=qONCevOTVA89K7vFJe-Bcc903lHsKDg6s661pTHCF2k,7682
 fbgemm_gpu/quantize_utils.py,sha256=pnZCkIeYxPnvwkIVsRdfPeGBLVXSpEdSsFLH2Ygk7D0,4005
 fbgemm_gpu/split_embedding_configs.py,sha256=Y3fJLHh4ffO6v_iKGc2MbBQTu8yFIMExEG_VYNW7rzI,5745
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=z1NugAsdcLO4nVFa_DJlOZHahmEdrBELi15ywFdaP3U,6661
@@ -28,11 +28,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py,sha256=pj1YxIVFTAngmyECHntbkrxiuquQk-rOP5hi3JnNmMc,3370
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py,sha256=dU1NN9KggZL-nOLY6lArLEMU2TTFSPVGGwoex3IN2UE,3370
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py,sha256=XRgP_N9mHwg5RLpDhtDIcogDHqY5Gw2C04QH4-W0Tk4,5005
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=C69JVjrCdRnkCGZq_KYJ1WXuj24z4nPWCpsezICsoXI,7014
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_weight_decay.py,sha256=OUATcloIxrOdnU_S0gcwiJbP95mtLX93hlYyqhNcdSc,3105
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_weighted_adagrad.py,sha256=UV7PGpsmOjbsPprmk3z-xTnkrEl4JkWl216o-V3T4YI,4961
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=7E-kNXqHV4_P0Cl6Zq8cRpKZFaHMAtS6x8r4Yq1PLJo,4250
-fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/METADATA,sha256=Frp9DiXwoGRM8Xlfn2q-NBtZgTX1BE4DC8a3ldTiC7A,2934
-fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
-fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2023.6.21.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/METADATA,sha256=KA3WRGiJlu7LnfjYTLBMgNalvILkU09UKlIxRiMnJZU,2934
+fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/WHEEL,sha256=uNTrmykJsfnOiRowEmEAgdbSsr7BScgAFZq1d9YxSqA,105
+fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2023.6.22.dist-info/RECORD,,
```

