add_executable(test_aead_aes256gcm
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/aead_aes256gcm.c
)
target_link_libraries(test_aead_aes256gcm
    sodium
)
target_include_directories(test_aead_aes256gcm
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_aead_aes256gcm
    COMMAND test_aead_aes256gcm
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_aead_aes256gcm2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/aead_aes256gcm2.c
)
target_link_libraries(test_aead_aes256gcm2
    sodium
)
target_include_directories(test_aead_aes256gcm2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_aead_aes256gcm2
    COMMAND test_aead_aes256gcm2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_aead_chacha20poly1305
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/aead_chacha20poly1305.c
)
target_link_libraries(test_aead_chacha20poly1305
    sodium
)
target_include_directories(test_aead_chacha20poly1305
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_aead_chacha20poly1305
    COMMAND test_aead_chacha20poly1305
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_aead_chacha20poly13052
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/aead_chacha20poly13052.c
)
target_link_libraries(test_aead_chacha20poly13052
    sodium
)
target_include_directories(test_aead_chacha20poly13052
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_aead_chacha20poly13052
    COMMAND test_aead_chacha20poly13052
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_aead_xchacha20poly1305
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/aead_xchacha20poly1305.c
)
target_link_libraries(test_aead_xchacha20poly1305
    sodium
)
target_include_directories(test_aead_xchacha20poly1305
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_aead_xchacha20poly1305
    COMMAND test_aead_xchacha20poly1305
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth.c
)
target_link_libraries(test_auth
    sodium
)
target_include_directories(test_auth
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth
    COMMAND test_auth
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth2.c
)
target_link_libraries(test_auth2
    sodium
)
target_include_directories(test_auth2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth2
    COMMAND test_auth2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth3.c
)
target_link_libraries(test_auth3
    sodium
)
target_include_directories(test_auth3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth3
    COMMAND test_auth3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth5
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth5.c
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/quirks.h
)
target_link_libraries(test_auth5
    sodium
)
target_include_directories(test_auth5
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth5
    COMMAND test_auth5
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth6
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth6.c
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/quirks.h
)
target_link_libraries(test_auth6
    sodium
)
target_include_directories(test_auth6
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth6
    COMMAND test_auth6
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_auth7
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/auth7.c
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/quirks.h
)
target_link_libraries(test_auth7
    sodium
)
target_include_directories(test_auth7
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_auth7
    COMMAND test_auth7
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box.c
)
target_link_libraries(test_box
    sodium
)
target_include_directories(test_box
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box
    COMMAND test_box
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box2.c
)
target_link_libraries(test_box2
    sodium
)
target_include_directories(test_box2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box2
    COMMAND test_box2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box7
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box7.c
)
target_link_libraries(test_box7
    sodium
)
target_include_directories(test_box7
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box7
    COMMAND test_box7
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box8
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box8.c
)
target_link_libraries(test_box8
    sodium
)
target_include_directories(test_box8
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box8
    COMMAND test_box8
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box_easy
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box_easy.c
)
target_link_libraries(test_box_easy
    sodium
)
target_include_directories(test_box_easy
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box_easy
    COMMAND test_box_easy
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box_easy2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box_easy2.c
)
target_link_libraries(test_box_easy2
    sodium
)
target_include_directories(test_box_easy2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box_easy2
    COMMAND test_box_easy2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box_seal
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box_seal.c
)
target_link_libraries(test_box_seal
    sodium
)
target_include_directories(test_box_seal
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box_seal
    COMMAND test_box_seal
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_box_seed
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/box_seed.c
)
target_link_libraries(test_box_seed
    sodium
)
target_include_directories(test_box_seed
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_box_seed
    COMMAND test_box_seed
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_chacha20
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/chacha20.c
)
target_link_libraries(test_chacha20
    sodium
)
target_include_directories(test_chacha20
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_chacha20
    COMMAND test_chacha20
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_codecs
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/codecs.c
)
target_link_libraries(test_codecs
    sodium
)
target_include_directories(test_codecs
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_codecs
    COMMAND test_codecs
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core_ed25519
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core_ed25519.c
)
target_link_libraries(test_core_ed25519
    sodium
)
target_include_directories(test_core_ed25519
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core_ed25519
    COMMAND test_core_ed25519
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core1
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core1.c
)
target_link_libraries(test_core1
    sodium
)
target_include_directories(test_core1
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core1
    COMMAND test_core1
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core2.c
)
target_link_libraries(test_core2
    sodium
)
target_include_directories(test_core2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core2
    COMMAND test_core2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core3.c
)
target_link_libraries(test_core3
    sodium
)
target_include_directories(test_core3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core3
    COMMAND test_core3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core4
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core4.c
)
target_link_libraries(test_core4
    sodium
)
target_include_directories(test_core4
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core4
    COMMAND test_core4
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core5
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core5.c
)
target_link_libraries(test_core5
    sodium
)
target_include_directories(test_core5
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core5
    COMMAND test_core5
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_core6
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/core6.c
)
target_link_libraries(test_core6
    sodium
)
target_include_directories(test_core6
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_core6
    COMMAND test_core6
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_ed25519_convert
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/ed25519_convert.c
)
target_link_libraries(test_ed25519_convert
    sodium
)
target_include_directories(test_ed25519_convert
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_ed25519_convert
    COMMAND test_ed25519_convert
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_generichash
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/generichash.c
)
target_link_libraries(test_generichash
    sodium
)
target_include_directories(test_generichash
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_generichash
    COMMAND test_generichash
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_generichash2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/generichash2.c
)
target_link_libraries(test_generichash2
    sodium
)
target_include_directories(test_generichash2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_generichash2
    COMMAND test_generichash2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_generichash3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/generichash3.c
)
target_link_libraries(test_generichash3
    sodium
)
target_include_directories(test_generichash3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_generichash3
    COMMAND test_generichash3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_hash
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/hash.c
)
target_link_libraries(test_hash
    sodium
)
target_include_directories(test_hash
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_hash
    COMMAND test_hash
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_hash3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/hash3.c
)
target_link_libraries(test_hash3
    sodium
)
target_include_directories(test_hash3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_hash3
    COMMAND test_hash3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_kdf
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/kdf.c
)
target_link_libraries(test_kdf
    sodium
)
target_include_directories(test_kdf
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_kdf
    COMMAND test_kdf
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_keygen
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/keygen.c
)
target_link_libraries(test_keygen
    sodium
)
target_include_directories(test_keygen
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_keygen
    COMMAND test_keygen
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_kx
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/kx.c
)
target_link_libraries(test_kx
    sodium
)
target_include_directories(test_kx
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_kx
    COMMAND test_kx
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_metamorphic
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/metamorphic.c
)
target_link_libraries(test_metamorphic
    sodium
)
target_include_directories(test_metamorphic
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_metamorphic
    COMMAND test_metamorphic
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_misuse
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/misuse.c
)
target_link_libraries(test_misuse
    sodium
)
target_include_directories(test_misuse
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_misuse
    COMMAND test_misuse
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_onetimeauth
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/onetimeauth.c
)
target_link_libraries(test_onetimeauth
    sodium
)
target_include_directories(test_onetimeauth
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_onetimeauth
    COMMAND test_onetimeauth
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_onetimeauth2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/onetimeauth2.c
)
target_link_libraries(test_onetimeauth2
    sodium
)
target_include_directories(test_onetimeauth2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_onetimeauth2
    COMMAND test_onetimeauth2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_onetimeauth7
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/onetimeauth7.c
)
target_link_libraries(test_onetimeauth7
    sodium
)
target_include_directories(test_onetimeauth7
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_onetimeauth7
    COMMAND test_onetimeauth7
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_pwhash_argon2i
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/pwhash_argon2i.c
)
target_link_libraries(test_pwhash_argon2i
    sodium
)
target_include_directories(test_pwhash_argon2i
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_pwhash_argon2i
    COMMAND test_pwhash_argon2i
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_pwhash_argon2id
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/pwhash_argon2id.c
)
target_link_libraries(test_pwhash_argon2id
    sodium
)
target_include_directories(test_pwhash_argon2id
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_pwhash_argon2id
    COMMAND test_pwhash_argon2id
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_pwhash_scrypt
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/pwhash_scrypt.c
)
target_link_libraries(test_pwhash_scrypt
    sodium
)
target_include_directories(test_pwhash_scrypt
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_pwhash_scrypt
    COMMAND test_pwhash_scrypt
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_pwhash_scrypt_ll
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/pwhash_scrypt_ll.c
)
target_link_libraries(test_pwhash_scrypt_ll
    sodium
)
target_include_directories(test_pwhash_scrypt_ll
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_pwhash_scrypt_ll
    COMMAND test_pwhash_scrypt_ll
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_randombytes
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/randombytes.c
)
target_link_libraries(test_randombytes
    sodium
)
target_include_directories(test_randombytes
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_randombytes
    COMMAND test_randombytes
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult.c
)
target_link_libraries(test_scalarmult
    sodium
)
target_include_directories(test_scalarmult
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult
    COMMAND test_scalarmult
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult_ed25519
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult_ed25519.c
)
target_link_libraries(test_scalarmult_ed25519
    sodium
)
target_include_directories(test_scalarmult_ed25519
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult_ed25519
    COMMAND test_scalarmult_ed25519
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult2.c
)
target_link_libraries(test_scalarmult2
    sodium
)
target_include_directories(test_scalarmult2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult2
    COMMAND test_scalarmult2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult5
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult5.c
)
target_link_libraries(test_scalarmult5
    sodium
)
target_include_directories(test_scalarmult5
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult5
    COMMAND test_scalarmult5
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult6
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult6.c
)
target_link_libraries(test_scalarmult6
    sodium
)
target_include_directories(test_scalarmult6
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult6
    COMMAND test_scalarmult6
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult7
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult7.c
)
target_link_libraries(test_scalarmult7
    sodium
)
target_include_directories(test_scalarmult7
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult7
    COMMAND test_scalarmult7
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_scalarmult8
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/scalarmult8.c
)
target_link_libraries(test_scalarmult8
    sodium
)
target_include_directories(test_scalarmult8
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_scalarmult8
    COMMAND test_scalarmult8
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox.c
)
target_link_libraries(test_secretbox
    sodium
)
target_include_directories(test_secretbox
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox
    COMMAND test_secretbox
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox2.c
)
target_link_libraries(test_secretbox2
    sodium
)
target_include_directories(test_secretbox2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox2
    COMMAND test_secretbox2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox7
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox7.c
)
target_link_libraries(test_secretbox7
    sodium
)
target_include_directories(test_secretbox7
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox7
    COMMAND test_secretbox7
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox8
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox8.c
)
target_link_libraries(test_secretbox8
    sodium
)
target_include_directories(test_secretbox8
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox8
    COMMAND test_secretbox8
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox_easy
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox_easy.c
)
target_link_libraries(test_secretbox_easy
    sodium
)
target_include_directories(test_secretbox_easy
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox_easy
    COMMAND test_secretbox_easy
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretbox_easy2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretbox_easy2.c
)
target_link_libraries(test_secretbox_easy2
    sodium
)
target_include_directories(test_secretbox_easy2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretbox_easy2
    COMMAND test_secretbox_easy2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_secretstream
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/secretstream.c
)
target_link_libraries(test_secretstream
    sodium
)
target_include_directories(test_secretstream
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_secretstream
    COMMAND test_secretstream
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_shorthash
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/shorthash.c
)
target_link_libraries(test_shorthash
    sodium
)
target_include_directories(test_shorthash
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_shorthash
    COMMAND test_shorthash
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sign
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sign.c
)
target_link_libraries(test_sign
    sodium
)
target_include_directories(test_sign
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sign
    COMMAND test_sign
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_siphashx24
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/siphashx24.c
)
target_link_libraries(test_siphashx24
    sodium
)
target_include_directories(test_siphashx24
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_siphashx24
    COMMAND test_siphashx24
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sodium_core
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sodium_core.c
)
target_link_libraries(test_sodium_core
    sodium
)
target_include_directories(test_sodium_core
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sodium_core
    COMMAND test_sodium_core
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sodium_utils
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sodium_utils.c
)
target_link_libraries(test_sodium_utils
    sodium
)
target_include_directories(test_sodium_utils
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sodium_utils
    COMMAND test_sodium_utils
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sodium_utils2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sodium_utils2.c
)
target_link_libraries(test_sodium_utils2
    sodium
)
target_include_directories(test_sodium_utils2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sodium_utils2
    COMMAND test_sodium_utils2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sodium_utils3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sodium_utils3.c
)
target_link_libraries(test_sodium_utils3
    sodium
)
target_include_directories(test_sodium_utils3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sodium_utils3
    COMMAND test_sodium_utils3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_sodium_version
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/sodium_version.c
)
target_link_libraries(test_sodium_version
    sodium
)
target_include_directories(test_sodium_version
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_sodium_version
    COMMAND test_sodium_version
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_stream
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/stream.c
)
target_link_libraries(test_stream
    sodium
)
target_include_directories(test_stream
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_stream
    COMMAND test_stream
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_stream2
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/stream2.c
)
target_link_libraries(test_stream2
    sodium
)
target_include_directories(test_stream2
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_stream2
    COMMAND test_stream2
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_stream3
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/stream3.c
)
target_link_libraries(test_stream3
    sodium
)
target_include_directories(test_stream3
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_stream3
    COMMAND test_stream3
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_stream4
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/stream4.c
)
target_link_libraries(test_stream4
    sodium
)
target_include_directories(test_stream4
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_stream4
    COMMAND test_stream4
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_verify1
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/verify1.c
)
target_link_libraries(test_verify1
    sodium
)
target_include_directories(test_verify1
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_verify1
    COMMAND test_verify1
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)

add_executable(test_xchacha20
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/cmptest.h
    ${PROJECT_SOURCE_DIR}/libsodium/test/default/xchacha20.c
)
target_link_libraries(test_xchacha20
    sodium
)
target_include_directories(test_xchacha20
    PRIVATE
        ${PROJECT_SOURCE_DIR}/libsodium/test/quirks/
)
add_test(
    NAME test_xchacha20
    COMMAND test_xchacha20
    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}/libsodium/test/default
)
